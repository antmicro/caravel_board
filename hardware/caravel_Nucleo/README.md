# Caravel Nucleo

![Caravel Nucleo](./img/caravel-nucleo.png)

### Overview

This repository contains open hardware design files for a expansion board compatible with [STM32 Nucleo-144 boards](https://www.st.com/en/evaluation-tools/stm32-nucleo-boards.html).\
This board connects IO signals from the STM32 MCU located on the Nucleo-144 board to an open hardware [Caravel](https://github.com/efabless/caravel_board).\
The Caravel breakout board allows testing ASIC designs prepared for Multi Project Wafer (MPW) shuttles and fabricated with one of the available open Process Design Kits (PDKs).

You can learn more about Open Shuttle Program by visiting this [link](https://efabless.com/open_shuttle_program).

The Caravel Nucleo board routes the interfaces from Caravel and provides the necessary power buses.
The design files were prepared in KiCad 6. This design is currently a Work in Progress (WiP).

## Project structure

The main repository directory contains KiCad PCB project files, and a README.
The remaining files are stored in the following directories:

* `lib` - contains the KiCad 6 component libraries
* `doc` - contains generated schematics and other documentation
* `img` - contains graphics for this README

## Key features

* Caravel-breakout testbed slot with optional FlexyPins
* `ST morpho` compatible
* USB for MPRJ SPI/UART debug
* SPI Flash connected to Caravel and Morpho connector
* Dedicated 10MHz oscillator
* Dual LDO with fixed and I2C controlled feedback (selectable)
