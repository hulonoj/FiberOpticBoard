# Fiber Optic Based Signal Replicator

A high-speed hardware system designed to transmit and replicate electrical signals over long distances using fiber optics with minimal latency.

## Overview

This project consists of two custom PCB systems designed for high-speed signal replication across fiber:

- **Transmitter/Receiver Board:** FPGA-based PCB for protocol-agnostic electrical signal replication over fiber with ~30 ns latency.
- **Motor Controller Board:** STM32-based H-Bridge driver interfaced via I2C through the fiber optic system.

The design demonstrates a full end-to-end communication system without electrical coupling, ideal for applications where noise isolation or long-distance communication is required.

## Features

- Custom fiber optic communication protocol with latency < 30 ns
- Supports arbitrary digital signal formats (protocol-agnostic)
- Isolated end-to-end data replication
- STM32 motor controller with I2C command input
- Integrated H-Bridge for direct motor control

## Photos

Fiber Optic Board mounted on top of a motor controller board.

<img src="Photos/FinishedBoard.jpg" width="500" height="500" />

Half-Assembled Fiber Optic Board

<img src="Photos/FinishedBoardoFiberOpt.jpg" width="700" height="400" />

Schematic
![Schematic](Photos/Fib_PCBSchematic.png)

Layout
![Layout](Photos/3dViewKiCadTop.png)

> 📸 *Replace these image filenames with your actual photo filenames in the `photos/` directory.*

## Files

- `schematics/` — Schematic design files
- `layout/` — PCB layout (Gerbers, board files)
- `bom/` — Bill of Materials
- `firmware/` — Embedded code for STM32
- `photos/` — Assembly and demo images
