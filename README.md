# Bilbao Maker Faire October 2018 FPGA beginner's workshop 
Shortlink to this documentation: [http://bit.ly/bbmf-fpga](http://bit.ly/bbmf-fpga)

Using the [IceBreaker board](https://github.com/icebreaker-fpga/icebreaker)
Soon to be available on [CrowdSupply](https://www.crowdsupply.com/1bitsquared/icebreaker-fpga)

![pinout](images/icebreaker-v1-0a-legend.jpg)

## Setup

* Install [IceStudio](https://github.com/FPGAwars/icestudio#installation)
* Install the [workshop package](https://github.com/mattvenn/collection-bilbao-makerfaire-2018/archive/0.1.zip)

## Challenges

### LEDS on

connect the boards LEDs to the 1 and 0 bits.

Solution: -> LEDS -> simple

Use more blocks to turn on other LEDs on the board.

### LEDs blinking

In the default collection, use the logic -> sequential -> PrescalarN block to flash an LED

### Buttons

Instead of using a 1 or 0 bit block, use a button to turn on and off an LED

### Button combo

combination of buttons to light LED

In the default collection, use Logic -> Gate -> And and Or to build a circuit that turns
on an LED when button 1 AND (button 2 OR button 3) is pressed.

Solution: Examples -> Buttons -> button logic

### All LEDs blinking at different rates

In the Bilbao collection, use the 8bit compare to flash multiple LEDs at different rates.

Solution: Examples -> LED -> different rates

### LEDs counting

In the Bilbao collection, use the Counter -> 4bit counter to count up to 16 in binary using 4 of the LEDs.

Solution: Examples -> LED -> counter

### LED sequencing

In the Bilbao colleciton, use the Counter -> 8bit compare block to make a sequence of LEDs.

LED 1 flashes 3 times, LED 2 turns on. LED 1 flashes 3 times, LED 2 turns off.

Solution: Examples -> LED -> led sequence

### VGA
