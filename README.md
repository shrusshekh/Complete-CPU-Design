# COE608 Lab 6 – Complete CPU Design with ALU and Control Unit

This project was developed as part of the **COE608 – Computer Organization & Architecture** course at **Toronto Metropolitan University**, aiming to design, simulate, and implement a **basic CPU** using VHDL and Quartus 16.0. 

---

## 🧠 Project Summary

The CPU includes a fully functional **Arithmetic Logic Unit (ALU)**, a **Control Unit** based on a Finite State Machine (FSM), and memory components. The system is capable of executing basic arithmetic and logical operations, driven by opcode inputs generated through a decoder linked to the FSM states. The output is displayed via waveform simulation (both timing and functional waveform simulations). 

---

## 🔧 Key Components

- **ALU Core** (`alu.vhd`)  
  Supports multiple operations including addition, subtraction, bitwise logic, shifting, and conditional functions based on opcode.

- **Control Unit** (`Control_NEW.vhd`, `control.vhd.bak`)  
  Implements FSM logic to generate state transitions and control signals.

- **Data Path & Memory** (`Data_Path.vhd`, `data_mem.vhd`)  
  Handles operand routing and temporary storage, connecting registers and the ALU.

- **Adders & Logic Modules**  
  - `adder4.vhd`, `adder16.vhd`, `adder32.vhd`  
  - `LZE.vhd`, `UZE.vhd`, `RED.vhd` (zero-extend and reduction logic)

- **Top-Level CPU Design** (`cpu1.vhd`, `CPU_TEST_Sim.vhd`)  
  Combines all subcomponents for final simulation and testing.

---

## 🧪 Simulation

- Waveform testbench: `CPU_TEST_Sim.vwf`
- Simulation performed in Quartus Prime Waveform Editor
- Output: `Result` value from the ALU is observed and verified through simulation cycles driven by the FSM

---
