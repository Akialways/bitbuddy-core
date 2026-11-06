# BitBuddy Core

An early-stage open-source **ESP32-C3 digital pet** project exploring expressive OLED faces, motion-based reactions, sound effects, and eventually Bluetooth interactions.

> **Status: prototype / work in progress.** This repository is a documentation and development starting point. It is not a finished firmware release.

## Project goals

- Compact digital pet keychain (target enclosure approximately 45–50 mm square)
- Expressive animations on a 0.96-inch 128×64 I²C OLED
- Gesture and tilt reactions using an MPU6050
- Simple audio feedback with a buzzer
- Future battery-powered operation, Bluetooth interactions, and minigames

## Prototype hardware

| Part | Purpose | Status |
| --- | --- | --- |
| ESP32-C3 Super Mini | Main controller | Prototype hardware |
| 0.96-inch I²C OLED | Pixel face | Basic display tested |
| MPU6050 | Movement sensing | Basic sensor test reported |
| Buzzer | Sound feedback | Basic buzzer test reported |
| Li-Po cell and charging module | Portable power | Integration pending |
| 3D-printed enclosure | Physical housing | Design in progress |

**Important:** Previous breadboard tests are not yet published as reproducible firmware. Firmware and schematics will be added after verification.

## Documentation

- [Prototype notes and tentative pin mapping](docs/hardware.md)
- [Roadmap](docs/roadmap.md)
- [Contributing](CONTRIBUTING.md)

## Safety and licensing

This is experimental electronics. Verify voltage levels, polarity, charging-module specifications, and battery protection before assembly. Do not connect a Li-Po cell directly to ESP32 GPIO pins.

All original material in this starter repository is available under the MIT License. Third-party designs, firmware, and proprietary assets are not included.
