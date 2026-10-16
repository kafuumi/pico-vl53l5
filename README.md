# pico-vl53l5

A Raspberry Pi Pico SDK port of the VL53L5CX multi-zone Time-of-Flight sensor
driver for RP2040 and RP2350 microcontrollers.

> [!IMPORTANT]
> This project is currently under development. The existing platform layer and
> examples are still based on ESP-IDF and have not yet been fully ported to the
> Raspberry Pi Pico SDK.

## Overview

This project aims to provide VL53L5CX support for boards based on:

- RP2040, including Raspberry Pi Pico and Pico W
- RP2350, including Raspberry Pi Pico 2 and Pico 2 W

The port will replace the ESP-IDF platform-specific implementation with
Raspberry Pi Pico SDK equivalents for I2C communication, GPIO control, timing,
and example applications.

## Project Status

The RP2040/RP2350 port is a work in progress.

Planned work includes:

- Implementing the platform abstraction with the Raspberry Pi Pico SDK
- Supporting hardware I2C communication
- Supporting optional sensor reset through GPIO
- Porting the example applications
- Adding CMake integration for Pico SDK projects
- Testing on RP2040 and RP2350 hardware

## Upstream Project

This project is based on the following ESP-IDF VL53L5CX library:

- [RJRP44/VL53L5CX-Library](https://github.com/RJRP44/VL53L5CX-Library)

The upstream project is an ESP32 adaptation of STMicroelectronics' VL53L5CX
Ultra Lite Driver.

## Sensor Documentation

For details about the VL53L5CX sensor and its Ultra Lite Driver, refer to the
official STMicroelectronics resources:

- [VL53L5CX product page](https://www.st.com/en/imaging-and-photonics-solutions/vl53l5cx.html)
- [VL53L5CX Ultra Lite Driver](https://www.st.com/en/embedded-software/stsw-img023.html)

## License

This project is distributed under the BSD 3-Clause License. See
[LICENSE](LICENSE) for details.

The VL53L5CX driver sources may also contain copyright notices and licensing
terms from STMicroelectronics and the upstream project.
