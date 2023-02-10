# Air mass meter input

air mass meter -> voltage divider -> rca91535 -> 8253 clock2 -> mcu

AMM/MAF input processing is done mostly in hardware. The differential signal from the AMM comes in on pins 7(+) and 6(-). The + signal enters a voltage divider that takes the raw voltage 1.25-4.5?v to 1.1-3.0v. This then enters the RCA 91535 chip and leaves as a frequency signal proportional to the amount of air that has passed through the AMM between the current RPM strobe and the last. 
