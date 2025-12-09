---
title: Bill of Materials
tags:
- tag1
- tag2
---


## Overview
This Bill of Materials (BOM) supports a custom microcontroller-based emitter and detector sensing system designed around the PIC18F57Q43. The circuit measures distance using two OPB732 sensors, amplifies and conditions signals with a Microchip MCP6004 op amp, and regulates power through an L7805ABV 5 V linear regulator. A L7805ABV shift register manages serial-to-parallel data control, while standard resistors and capacitors provide biasing, filtering, and power stability. All components are readily available through Digi-Key and are suitable for prototyping or small-scale production.


## Bill of Materials 

| **Part Name/Description** | **Qty** | **Unit Cost** | **Total Cost** | **Manufacturer** | **Manufacturer #** | **Vendor Link** | **Datasheet Link** | **# Ordered** | **Date Ordered** | **# Receiver** | **Schematic Reference Designators** |
|:--------------------|:----|:---------------|:-----|:--------|:-----|:-----|:----|:-----|:-----|:-----|:-----|
| Microchip PIC18F57Q43 Curiosity Nano Dev Kit | 1 | $9.99 | $9.99 | Microchip | DM164150 | [Microchip Direct](https://www.microchipdirect.com/dev-tools/DM164150?productLoaded=true&allDevTools=true) | [Datasheet](https://ww1.microchip.com/downloads/aemDocuments/documents/MCU08/ProductDocuments/DataSheets/PIC18F27-47-57Q43-Microcontroller-Data-Sheet-XLP-DS40002147.pdf) | **1** | **NA** | **1** | U1 |
| Reflective Emitter and Detector Sensor (OPB732) | 2 | $4.61 | $13.83 | TT Electronics/Optek Technology | 365-1691-ND | [DigiKey](https://www.digikey.com/en/products/detail/adafruit-industries-llc/4007/9857020) | [Datasheet](https://www.ttelectronics.com/TTElectronics/media/ProductFiles/Datasheet/OPB732.pdf) | **3** | **8/12/2025** | **3** | U3, U4 |
| Op Amp, Four, Rail-to-Rail, 5 V | 1 | $0.59 | $0.59 | Microchip Technology | MCP6004-I/P | [DigiKey](https://www.digikey.com/en/products/detail/microchip-technology/MCP6004-I-P/523060) | [Datasheet](https://ww1.microchip.com/downloads/aemDocuments/documents/OTH/ProductDocuments/DataSheets/21969b.pdf) | **2** | **8/12/2025** | **2** | MCP6004_OPAMP1 |
| Linear Voltage Regulator, 5 V, 1.5 A, TO-220 | 1 | $0.59 | $0.59 | STMicroelectronics | L7805ABV | [DigiKey](https://www.digikey.com/en/products/detail/stmicroelectronics/L7805ABV/634711) | [Datasheet](https://www.st.com/resource/en/datasheet/l7805.pdf) | **2** | **8/12/2025** | **2**  | U2 |
| 100 kΩ Resistor, ¼ W | 4 | $0.10 | $0.40 | Yageo | MFR-25FBF52-100K | PRLTA 109 | n/a | NA | NA | NA | R8, R10, R17, R18 |
| 10 kΩ Resistor, ¼ W | 3 | $0.10 | $0.30 | Yageo | MFR-25FBF52-10K | PRLTA 109 | n/a | NA | NA | NA | R5, R7, R16 |
| 2 kΩ Resistor, ¼ W | 4 | $0.10 | $0.40 | Yageo | MFR-25FBF52-2K | PRLTA 109 | n/a | NA | NA | NA | R1, R2, R13, R14 |
| 1 kΩ Resistor, ¼ W | 3 | $0.10 | $0.30 | Yageo | MFR-25FBF52-1K | PRLTA 109 | n/a | NA | NA | NA | R3, R4, R15 |
| 220 kΩ Resistor, ¼ W | 4 | $0.10 | $0.40 | Yageo | MFR-25FBF52-220K | PRLTA 109 | n/a | NA | NA | NA | R11, R12, R19, R20 |
| 220 Ω Resistor, ¼ W | 2 | $0.10 | $0.20 | Yageo | MFR-25FBF52-220K | PRLTA 109 | n/a | NA | NA | NA | R6, R9 |
| 0.1 µF Ceramic Capacitor, ±10%, X7R, 50 V, 0805 package | 3 | $0.28 | $0.84 | KEMET | C0805F104K5RACTU | PRLTA 109 | n/a | NA | NA | NA | C1, C2, C3, C4, C5 |
