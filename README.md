# Raspberry Pi 7-Segment Counter

**Platform:** Raspberry Pi · Python GPIO · 74HC595 shift register · 5011AS common-cathode display  
**Status:** Wiring reference located; original user-written Python source and physical prototype evidence still need to be confirmed.

## Project overview

The learning project is to display the digits 0–9 on a single 5011AS seven-segment display. The Raspberry Pi sends serial data to a 74HC595 shift register, which controls the display segments.

## Wiring reference recorded in the Library

### Raspberry Pi to 74HC595

| Raspberry Pi physical pin | BCM GPIO / signal | 74HC595 pin |
|---|---|---|
| 2 | 5 V | 16 (VCC) |
| 6 | GND | 8 (GND), 13 (OE) |
| 4 | 5 V | 10 (SRCLR) |
| 11 | GPIO 17 / DATA | 14 (SER) |
| 12 | GPIO 18 / LATCH | 12 (RCLK) |
| 13 | GPIO 27 / CLOCK | 11 (SRCLK) |

### 74HC595 to 5011AS

Outputs QA–QG connect to segments a–g through individual 220 Ω resistors. The 5011AS common-cathode pins connect to ground. The decimal point is unused in the recorded wiring reference.

**Important:** Confirm the exact display pinout against the component datasheet before powering the circuit. Use one current-limiting resistor per segment.

## Repository contents

- `docs/raspberry-pi-74hc595-5011as-pinout.md` — transcription of the Library wiring reference.
- Original project source code and breadboard photographs have not yet been identified for upload.

## Verification status

- [x] Wiring reference located.
- [ ] Original Python counter source recovered.
- [ ] Fritzing diagram added.
- [ ] Prototype photographs added.
- [ ] Digits 0–9 tested and recorded.

## Author

Thabiso Ndlovu
