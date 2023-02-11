# Software Overview
## MCS-48 8bit Timer
Timer mode, Interrupt every 10ms, incremented every 57us

## MCS-48 External Interrupt
Input from 0141 RPM IC

## ADC 0809
### Inputs
* AN0 CO Pot
* AN1 Voltage
* AN2 Temp
* AN3 WOT Switch
* AN4 GND (starter/auto pnp)
* AN5 GND
* AN6 MAF -
* AN7 MAF +

## Programmable Interval Timer
### Timer 0:
Injector output
Mode 0 (Interrupt on count)
* CLK0 - MCU ALE strobe (559khz)
* OUT0 - Injector output
* GATE0 - NC (tied high)

### Timer 1:
Idle air control output
Mode 3 (square wave generator)
* CLK1 - MCU ALE strobe (559khz)
* OUT1 - IAC output
* GATE1 - ?

### Timer 2:
Air mass meter input from RCA 91535
Mode 3 (square wave generator)
* CLK2 - RCA 91535
* OUT2 - NC (floating)
* GATE2 - NC (tied high)
