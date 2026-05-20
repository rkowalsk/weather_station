# Environmental Monitoring Station

Simple Environmental Monitoring Station project based on an STM32F401RE Nucleo board and a BME280 sensor.

It reads temperature, humidity, and pressure data from the sensor and outputs the values over USB serial via the ST-Link virtual COM port.

## Context

I created this project to teach myself embedded engineering. The concept of this project is very unoriginal but my goal wasn't to change the world or create a viable commercial product.

## Features

- Reads temperature, humidity, and pressure from BME280 via I2C
- USB serial output via ST-Link (Virtual COM Port)
- Built with STM32CubeIDE / STM32 HAL

## Hardware

- STM32 NUCLEO-F401RE
- BME280 sensor module

## Software

- Written in C
- Uses the STM32's HAL and the BME280 sensor driver 
- CubeMX was used to generate the initialization code

## Build

Using `make`:

```bash
make
````

## Serial Output

Connect to the ST-Link virtual COM port:

* Baud rate: `115200`

Example output:

```text
Temperature: 22.7°C | Pressure: 97569Pa | Humidity: 45%
```

