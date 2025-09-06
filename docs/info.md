<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

This circuit is a step counter with a 7-segment display.

The Step button acts as the clock input. Each press increments the counter by one.

The Reset button clears the count back to zero.

The counter output goes through a decoder, which translates the binary value into the appropriate signals for the 7-segment display, showing the current count.

The resistor and 10k potentiometer are used as pull-downs or to stabilize the button input.
## How to test

Power the circuit with VCC.

Press the Reset button to ensure the display shows zero.

Press the Step button multiple times and observe the 7-segment display increase its value sequentially (0 → 1 → 2 …).

Press Reset again to check if the display returns to zero.

Verify that each step produces a consistent count without skipping or bouncing (debouncing might be needed if you see erratic values).

## External hardware

Power supply

Pushbuttons (Step and Reset).

Resistors / potentiometers for pull-down or pull-up stabilization.

7-segment display to visualize the counter output.

Optionally, a debouncing circuit (capacitor or Schmitt trigger) if button presses are unstable.
