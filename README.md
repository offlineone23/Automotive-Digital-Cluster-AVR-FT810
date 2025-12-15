# Automotive Digital Instrument Cluster (AVR + FT810)

## Overview
This project is a full digital instrument cluster designed and implemented as a real automotive replacement
for Peugeot 405 / Pars vehicles.

The system replaces the factory analog cluster with two 7" TFT LCDs driven by FT810 controllers,
fully controlled by an ATmega128 microcontroller over SPI.

## Key Features
- Dual 7" LCD (AT070TN92) driven by FT810
- Speed and RPM measurement using input capture
- Fuel level and temperature via ADC
- Non-volatile data storage (odometer, trip) using external memory
- Automotive-safe signal conditioning (voltage spikes, noise, ignition reset)
- Custom-designed PCB (Altium Designer)
- Custom UI graphics (3ds Max & Photoshop)

## Hardware
- Microcontroller: ATmega128
- Display Controller: FT810 (x2)
- Communication: SPI
- Power Supply: LM2576, XL6009, negative voltage generation
- Automotive signal conditioning circuits

## Software
- Bare-metal C (AVR-GCC / CodeVision)
- Timer, ADC, Input Capture
- SPI display driver
- Custom graphics rendering pipeline

## Status
Implemented, tested, and deployed on a real vehicle.
