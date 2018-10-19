# Bilbao Maker Faire October 2018 FPGA beginner's workshop 
Shortlink to this documentation: [http://bit.ly/bbmf-fpga](http://bit.ly/bbmf-fpga)

Using the [IceBreaker board](https://github.com/icebreaker-fpga/icebreaker)
Soon to be available on [CrowdSupply](https://www.crowdsupply.com/1bitsquared/icebreaker-fpga)

![pinout](images/icebreaker-v1-0a-legend.jpg)

## Setup

* Install [IceStudio](https://github.com/FPGAwars/icestudio#installation)
* Install the [workshop package](https://github.com/mattvenn/collection-bilbao-makerfaire-2018/archive/master.zip)

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

In the Bilbao collection, use the Counter -> 8bit compare block to make a sequence of LEDs.

LED 1 flashes 3 times, LED 2 turns on. LED 1 flashes 3 times, LED 2 turns off.

Solution: Examples -> LED -> led sequence

### red VGA

Load Examples -> VGA -> red

Upload onto the board and check the display shows a red screen.

The AND gates are used so that the red, green and blue outputs are only on when the active video signal is true.

Modify the 1s and 0s to change the colour to green and blue

### colour control

Instead of using the 1s and 0s to change the colours, use the 3 buttons.

Solution: Examples -> VGA -> buttons

### split colours

Make the bottom half of the screen blue.

In the Bilbao collection, use the Counter -> 10bit compare block to compare the y_px output of the VGA block with a parameter.
Use the more output of the compare block to drive the AND gate of the blue signal.

Solution: Examples -> VGA -> half blue

#### Advanced

* split the screen up in different ways
* use the x_px output of the VGA to do vertical splits

### colour sequence

* Use the PrescalarN and 8bit compare blocks to change the colours on the screen in a sequence.
* Use the px_clk output from the VGA block as the input to the PrescalarN block.

Solution: Examples -> VGA -> sequence

#### Advanced

* Use multiple compare blocks to animate different colours
* Split the outputs to get more colour control

### cross

* use a few 10bit compare blocks to draw a cross on the screen

Solution: Examples -> VGA -> cross

