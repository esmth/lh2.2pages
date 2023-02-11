# Fueling
## Main map
(insert photo)
The main fuel map is a 12bit 16x16 map with the x axis being RPM and y axis cylinder load from the RCA chip. 

## axis
Location 0xb16 (load), 0xb24 (RPM)

# location
* 0x300 - low 8 bits
* 0x900 - high 2 bits

## Decel Fuel Cut Off
Above X RPM and Y temperature, when idle pin is low, the ECU will cut all fuel. 

## Rev Limiter
Engine speed limiter. Stock 6200RPM, cuts fuel instantly.

