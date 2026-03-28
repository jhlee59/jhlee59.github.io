---
title: ID: API
---
To be edited 
# Hattie Camera Node API (Node ID 0x03)

This page defines the canonical API for the Hattie camera subsystem in the team daisy-chain architecture. All messages follow the 64-byte class protocol (bytes 0–3 prefix, 4–61 payload, 62–63 suffix).

Node ID: `0x03`  
Role: Camera / Sensors  

---

## Node Responsibilities

- Send telemetry packets with camera and sensor data.
- Receive configuration updates and telemetry requests.
- Forward messages not intended for this node downstream.
- Provide ACKs and error reporting for received commands.

---

## Message Types

### 1. `0x0003` — Telemetry Packet (Sent by Camera Node)

| Byte | Variable Name   | Type      | Min   | Max    | Example |
|------|----------------|-----------|-------|--------|---------|
| 6–7  | distance_mm    | uint16_t  | 0     | 5000   | 1200    |
| 8    | motion_detected| uint8_t   | 0     | 1      | 1       |

Status Flags:
- bit0 = Camera operational
- bit1 = Error present
- bit2 = Low battery

---

### 2. `0x0004` — ACK (Sent by Camera Node)

| Byte | Variable Name      | Type    | Min | Max | Example          |
|------|------------------|---------|-----|-----|-----------------|
| 6    | acked_msg_type    | uint8_t | 0   | 255 | 0x0FFF (low byte) |
| 7    | status            | uint8_t | 0=OK,1=ERROR | 0 | 0 |
| 8    | error_code        | uint8_t | 0   | 255 | 0 |
| 9–61 | message           | char[]  | N/A | N/A | "Config Applied" |

---

### 3. `0x0005` — Error / Event Log (Sent by Camera Node)

| Byte | Variable Name | Type      | Min | Max | Example          |
|------|---------------|-----------|-----|-----|-----------------|
| 6    | error_code    | uint8_t   | 1   | 255 | 0x02            |
| 7    | severity      | uint8_t   | 0=info,1=warn,2=error,3=fatal | 2 | 2 |
| 8–61 | message       | char[]    | N/A | N/A | "Camera overtemp" |

---

### 4. `0x0FFF` — Config Update (Received by Camera Node)

| Byte | Variable Name | Type      | Min | Max | Example                  |
|------|---------------|-----------|-----|-----|-------------------------|
| 6    | config_id     | uint8_t   | 0   | 255 | 0x01                    |
| 7    | data_len      | uint8_t   | 0   | 55  | 5                       |
| 8–(8+N-1)| config_data| uint8_t[] | N/A | N/A | [0x10,0x20,0x00,0x01,0xFF] |
| Remaining | reserved | uint8_t[] | 0   | 0xFF | 0 |

---

## Node Addressing

| Node  | ID    |
|-------|-------|
| Riley (MQTT Gateway) | 0x01 |
| Bryce (Motor Node)   | 0x02 |
| **Hattie (Camera / Sensors)** | 0x03 |
| Rylee (Controller Input) | 0x04 |
| Tim (Motor Node)     | 0x05 |
| Broadcast            | 0xFF |

---

## Routing Rules

1. If Destination ID = local node ID → consume packet.  
2. If Destination ID = 0xFF → broadcast and optionally respond.  
3. Otherwise → forward downstream.  
4. ACKs must be routed back to the Source ID.  
5. Preserve bytes 0–3 and 62–63 unchanged when forwarding.

---
