# ESP32 Snake Game with TFT Display

## Project Overview

This project implements the classic **Snake Game** using an ESP32 microcontroller, an analog joystick for control, and a 2.8-inch ILI9341 TFT LCD display for graphics.

The player controls the snake using the joystick. The goal is to eat the food appearing on the screen while avoiding collisions with the walls or the snake's own body.

## Hardware Components

* ESP32 Development Board
* ILI9341 2.8" TFT LCD Display
* Analog Joystick Module
* Jumper Wires

## Libraries Used

* Adafruit GFX Library
* Adafruit ILI9341
* SPI Library

## Display Specifications

| Feature      | Value            |
| ------------ | ---------------- |
| Controller   | ILI9341          |
| Resolution   | 320 × 240 pixels |
| Interface    | SPI              |
| Display Type | TFT LCD          |
| Color Depth  | 65K colors       |

## Pin Connections

### TFT Display to ESP32

| Display Pin | ESP32 Pin |
| ----------- | --------- |
| VCC         | 3.3V      |
| GND         | GND       |
| CS          | GPIO5     |
| DC          | GPIO2     |
| RESET       | GPIO4     |
| MOSI        | GPIO23    |
| SCK         | GPIO18    |
| LED         | 3.3V      |

Note: The MISO pin is not required because the ESP32 only sends data to the display.

### Joystick to ESP32

| Joystick Pin | ESP32 Pin |
| ------------ | --------- |
| VCC          | 3.3V      |
| GND          | GND       |
| VRX          | GPIO34    |
| VRY          | GPIO35    |

## How the Game Works

1. The snake moves continuously across the screen.
2. The joystick controls the direction of the snake.
3. Food appears randomly on the screen.
4. Each time the snake eats food, it grows longer.
5. The game ends if the snake hits the wall or its own body.

## Simulator

This project can be simulated using the **Wokwi online simulator**.

## Future Improvements

* Score display
* Increasing game speed
* Start screen
* High score memory
* Sound effects

## Author
V.Venkata Harinath
Diploma ECE SVGP TIRUPATI
Embedded Systems Project using ESP32 and TFT graphics.
