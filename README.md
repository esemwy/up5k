Upduino v2 examples with icestorm
====

Several demos showing how to use the `icestorm` toolchain with the
Upduino (ice40 UltraPlus 5k) FPGA dev board.

| Demo | Description |
|------|-------------|
| `blink` | Flash the RED LED in a pulse-pulse, pulse-pulse pattern |
| `pulse` | Smoothly ramp the RGB LED through a color change pattern |
| `serial` | Print a repeating message on the serial port at 3 Mbs |
| `seral-echo` | Read from the serial port, echo it back at 3 Mbs |
| `spram-demo` | Read from the serial port, buffer in SPRAM, echo it slowly |

To flash them, run `sudo make blink.flash`.
You will probably need to be root to flash the board and restore the
`/dev/ttyUSB0` device driver after `iceprog` switches it into SIO mode.


Schematics and pinout
====

Schematics for the upduino: https://github.com/gtjennings1/UPDuino_v2_0

![Upduino v2 pinout by Matt Mets](pinout.jpg)

