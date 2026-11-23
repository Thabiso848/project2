# Raspberry Pi – 74HC595 – 5011AS Pinout

This document records the connections in the Library file `Raspberry_Pi_74HC595_5011AS_Pinout.docx`.

## Raspberry Pi to 74HC595

| Raspberry Pi physical pin | Signal | 74HC595 pin |
|---|---|---|
| 2 | 5 V | 16 (VCC) |
| 6 | GND | 8 (GND), 13 (OE) |
| 4 | 5 V | 10 (SRCLR) |
| 11 / GPIO 17 | DATA | 14 (SER) |
| 12 / GPIO 18 | LATCH | 12 (RCLK) |
| 13 / GPIO 27 | CLOCK | 11 (SRCLK) |

## 74HC595 to 5011AS

| 74HC595 output | Display segment |
|---|---|
| QA (pin 15) | a |
| QB (pin 1) | b |
| QC (pin 2) | c |
| QD (pin 3) | d |
| QE (pin 4) | e |
| QF (pin 5) | f |
| QG (pin 6) | g |
| QH (pin 7) | DP — not connected |

Use an individual 220 Ω current-limiting resistor in series with each display segment. The 5011AS common-cathode pins connect to GND.

## Safety and verification

Check the manufacturer's datasheet and physical pin numbering before wiring. Do not assume the wiring is correct for a different display variant. Power down before changing connections.

**Evidence status:** This is a transcribed wiring reference, not proof of a tested working prototype.
