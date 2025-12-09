--- 
title: Hardware V2.0
tags:
- tag1
- tag2
---


The current hardware design functions properly, but several improvements would enhance the system's reliability and ease of maintenance. The most significant change would be to separate the design into two PCBs. Although the [schematic](https://jhlee59.github.io/04-Schematic/schematic/) places both sensors close together, the motion sensor and the depth sensor must be installed in physically different areas of the trash can. Keeping them on a single PCB requires long wire runs, which can introduce noise, make installation more challenging, and increase the likelihood of mechanical strain. Creating a “lid PCB” for the motion sensor and a “bin PCB” for the depth sensor would reduce wiring complexity and improve signal quality.

With each sensor on its own channel and its own board, the microcontroller no longer has to constantly handle overlapping signals or compensate for noise caused by long wiring runs. This reduces the chances of misreadings, unstable analog values, or incorrect triggering when switching between channels. Cleaner, more isolated inputs allow the code to use straightforward analog-to-digital reads and thresholds, eliminating the need for extra filtering, error-checking, or calibration routines. As a result, the software becomes easier to write, easier to debug, and far less prone to unexpected behavior during operation.

