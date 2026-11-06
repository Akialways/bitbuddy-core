# Prototype hardware notes

This is a work-in-progress reference, **not** a validated production schematic.

## Components

- ESP32-C3 Super Mini
- 0.96-inch 128 × 64 I²C OLED
- MPU6050 motion sensor
- Three-pin buzzer module
- Li-Po battery and a suitable charging/power system (integration pending)

## Previously tested wiring (verify before reproducing)

| Signal | ESP32-C3 GPIO |
| --- | --- |
| I²C SDA | GPIO4 |
| I²C SCL | GPIO5 |
| Buzzer control | GPIO3 |

The OLED was reported at I²C address `0x3C`. Scan the bus to verify peripheral addresses, especially the MPU6050, on your specific modules. Supply voltage and module pin markings must be checked before powering the circuit.

## Safety

Never connect a Li-Po cell directly to a GPIO pin. Verify charging-module protection, battery polarity, output rails, and available current. Do not assume a USB-C TP4056 module alone provides a regulated output compatible with every ESP32 board.

## Reproducibility

The original tested sketches have not yet been published or independently re-tested as a single integrated firmware build. Firmware, photos, and an electrical schematic will be added when validated.
