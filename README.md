# BYO8088
This is a modern implementation of the 8088 minimum mode SBC based on the one from Walter Fuller
as used in his book "Build Your Own Computer".

##Introduction
The orignal design as built in the book appears to have been done on a breadboard, so I took
the basic design and implemented it (partially) in an ECB (100mm x 160mm) format to take
advantage (ultimately) of various peripherals available in the Retrobrew Computer board
series.

##How is this version different?
As currently drawn, my reimplementation makes the following changes:

- Adds three 73LS373 drivers for the address bus in the event I want to expose those to
  the ECB connector (which right now is only for power).

- Removed the ADC0808 analog-to-digital converter.

- Used only one 82C55 I/O chip.

- Removed the RS-232 level shifters in favor of a header for a USB dongle.

- Added jumpers for the EPROM to allow for a flash-equivalent chip.

##Testing
As of now, this design is untested but I don't see why it wouldn't work.
