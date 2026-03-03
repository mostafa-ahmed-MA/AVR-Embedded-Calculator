# ATmega32 Embedded Systems Calculator

A high-performance digital calculator project designed using the AVR ATmega32 microcontroller. This project demonstrates interfacing between a microcontroller, a 4x4 matrix keypad, and a 16x2 LCD display to perform real-time arithmetic operations.

## Project Overview

This system is built to handle basic mathematical operations including addition, subtraction, multiplication, and division. The firmware is optimized for low-latency input processing and accurate LCD rendering.

## Hardware Components

The circuit is designed in Proteus and consists of:
- Microcontroller: ATmega32 (AVR Architecture)
- Display: 16x2 Alpha-Numeric LCD (LM016L)
- Input: 4x4 Matrix Keypad
- Power Source: 5V DC

## Circuit Schematic

The following image illustrates the connection between the ATmega32 pins and the peripherals:

![Circuit Diagram](Cap2222ture.PNG)

### Connection Mapping:
- PORTA (PA0 - PA7): Connected to LCD Data pins (D0 - D7) for 8-bit communication.
- PORTB (PB0, PB1, PB2): Connected to LCD Control pins (RS, RW, E).
- PORTD (PD0 - PD7): Connected to the 4x4 Keypad matrix (Rows and Columns).

## Simulation Demo

You can find the functional simulation of the project below:

![Project Animation](Animation.gif)

## Project Structure

The repository is organized as follows:
- code/: Contains the C/C++ source code and header files.
- calculator.pdprj: The Proteus design file for simulation.
- Animation.gif: A visual demonstration of the calculator in action.

## How to Run

1. Clone this repository to your local machine.
2. Open the 'calculator.pdprj' file using Proteus 8.0 or higher.
3. Load the .hex file (found in the code folder) into the ATmega32 component.
4. Run the simulation and use the keypad to perform calculations.

## Future Improvements
- Adding support for complex scientific functions (Sin, Cos, Tan).
- Implementing a history feature to store previous calculations.
- Upgrading to a 4-bit LCD communication mode to save I/O pins.