---
title: Microcontroller Code
---

## Overview

This is the code for the PCB to support two Reflective Optical Sensors. Detecting and reading an analog signal that the Op Amp then amplifies. The microcontroller translates this into a digital signal for two other microcontrollers to read. Two separate signals from two separate sensors to two separate other microcontrollers. Turning a Debug LED on until a signal is sensed and sent.

To read both sensors: 
      ADC_ConversionStart();
      while (!ADC_IsConversionDone()) ;
were used. 

```
#include "mcc_generated_files/system/system.h"
#include <stdio.h>

/*
    Main application
*/

int main(void)
{
    SYSTEM_Initialize();
    ADC_Initialize();
    UART1_Initialize();
    
    uint16_t resultM = 0;
    uint16_t resultD = 0;

    while(1)
    {
        
        
        
        ADC_ChannelSelect(0x04);     // RA4 = AN4
        __delay_us(10);
        ADC_ConversionStart();
        while (!ADC_IsConversionDone()) ;
        resultD = ADC_ConversionResultGet();

        
        printf("Motion=%u   Distance=%u\r\n", resultM, resultD);

        if(resultD > 720)
        {
            DEBUG_LED_SetLow();
            BLED_SetHigh();
            __delay_ms(10);
        }
        else
        {
            DEBUG_LED_SetHigh();
            BLED_SetLow();
            __delay_ms(10);
        }
      
        ADC_ChannelSelect(0x03);     // RA3 = AN3
        __delay_ms(10);
        ADC_ConversionStart();
        while (!ADC_IsConversionDone()) ;
        resultM = ADC_ConversionResultGet();

        if(resultM > 620)
    
        {
            DEBUG_LED_SetLow();
            RLED_SetHigh();
            BLED_SetLow();
            __delay_ms(10);
        }
        else
        {
            DEBUG_LED_SetHigh();
            RLED_SetLow();
            BLED_SetLow();
            __delay_ms(10);
        }

        __delay_ms(30);
    }

    return 0;
}
```

[2sensors.zip](https://github.com/user-attachments/files/23917806/2sensors.zip)
