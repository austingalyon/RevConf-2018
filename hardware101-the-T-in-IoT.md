Bryan Hughes, PHD
Nebrius

# Microcontrollers
- 3 types/groups

## Mini Computers
Raspberry Pi
- wireless module in top left (Under Raspberry logo)
- Processor under broadcom
- Multitude of OS's
  - Raspbian - Special flavor of Debian
  - Vanilla Ubuntu (? look into this)
  - Windows (?!?!)

- at idle draws 400 mA
  - 5000 mAh battery bank will last you ~7 hours

Tessel
- identical set of IO pins
- sell modules that are plug 'n play

Other Boards
- Intel
- Asus
- Others

## Tiny Brains
- can't run a full os
- battery power drain is significantly lower

Arduino Uno (~$30)
> had to have dev kits (couple hundred - couple thousand) prior to their creation
- 8 MHz

Huzzah (ESP8266)
- 16 MHz
- has wireless board built in

ESP12E (ESP8226)
- surface mounted board (used in ESP8226, mounted on the Huzzah)
- FCC certified module (3rd party) allows FCC license bypassing

*Board from picture controls LED Strips.*

## Amolyogous

krtkl Snickerdoodle
- processor
- Field-Programmable Gate Array (FPGA)
  - integrated circuit that you create

# Connections
General Purpose Input/Output (GPIO)
- On = Supply Voltge
  - 3v or 5v
  - referred to as VCC
- Off = 0v
  - referred to as Negative (in Batteries), Ground, or GND

Pulse Width Modulation
- on for certain period, off for rest.
- on for 1ms, off for 19ms

>use pwm to make dimmable LEDs
>use R, G, & B LEDs w/ PWM to create 16bit color

Universal Asynchronous Reciever/Transmitter (UART)
- Also known as Serial
- TXD - Transmit pin 
- RXD - Recieve Pin
- clock rates need to be synched

Inter-Integrated Circuit Bus (I^2C)
- SDA - Serial Data
- Microcontroller orchestrates and facilitates communications
- I2C has an official packet format
  - each packet has a header which includes an address
- Microcontroller has to ask for data to be able to recieve any
  - "Do you have anything for me?"
- SCL - Serial Clock
  - Provides Clock Reference
  - Ensures Clock Rate synchronization
- Have to send twice as much data as you need to read

Serial Peripheral Interface Bus (SPI)
- Much more complicated, but much faster reads
- MOSI - Master out, Slave in
- MISO - Master in, Slave out
- GPIOs indicate desire to send data
- data transmission over MOSI and MISO?
- 10s-100+ Mbps

# Software
*Examples in [Johnny-Five](johnny-five.io)*
*Pictures of examples on Phone*

Universal Ground
- Need to have 
- ensures off is the same accross the board

Clock Rate

*2nd pic, pressed = on, not pressed = off*