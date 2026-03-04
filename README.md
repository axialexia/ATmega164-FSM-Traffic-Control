# Smart Traffic Light System with Emergency Prioritization

## Project Overview
This project implements an intelligent traffic control system using the Atmel ATmega164 microcontroller.Designed for high-density urban areas, the system optimizes traffic flow through real-time sensor data and ensures safety by providing immediate priority to emergency vehicles (Ambulance, Fire, Police).

## Key Features
* **Finite State Machine (FSM):** Orchestrates 6 distinct operational states using sequential logic circuits (CLS).
* **Emergency Override Mode:** Features an immediate "Green Light" trigger for emergency vehicles via simulated radio signals (URG).
* **Adaptive Traffic Sensing:** Adjusts the Green phase duration (extending it by approx. 15s) when traffic sensors (IR/Pressure) detect high vehicle density.
* **Energy Efficiency:** Defaults to a power-saving Red state when no vehicle presence is detected.
* **Non-Blocking Logic:** Uses internal timers (tick-based) for precise state transitions:
  * Green: 10s
  * Yellow: 3s
  * Red: 10s

## Technical Specifications
* **Architecture:** Combinational Logic (CLC) for sensor processing and Sequential Logic (CLS) for state transitions.
* **Microcontroller:** ATmega164 (10.0 MHz Clock).
* **Development Environment:** CodeVisionAVR.
* **Inputs/Outputs:** Uses PORTB for LED signaling and PIND for sensor/button inputs.

## Documentation
For a full technical breakdown, logic tables, and state diagrams, please refer to the attached PDF:
* [📄 Technical Documentation (PDF)](Semafor_Inteligent_Prioritizare_Urgenta(1).pdf)
