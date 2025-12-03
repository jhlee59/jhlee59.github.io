---
title: Microcontroller Code
---

## Overview

This is the code for the PCB to support two Reflective Optical Sensors. Detecting and reading an analog signal that the Op Amp then amplifies. The microcontroller translates this into a digital signal for two other microcontrollers to read. Two separate signals from two separate sensors to two separate other microcontrollers. Turning a Debug LED on until a signal is sensed and sent.

To read both sensors: 
      ADC_ConversionStart();
      while (!ADC_IsConversionDone()) ;
were used. 

[2sensors.zip](https://github.com/user-attachments/files/23917806/2sensors.zip)
