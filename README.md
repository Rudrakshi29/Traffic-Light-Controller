# Traffic-Light-Controller
## Project Overview:
This project implements a Finite State Machine (FSM)-based traffic light controller for a two-way intersection using Verilog HDL. The design is simulated and verified using Xilinx Vivado. The controller cycles through traffic light states (Green → Yellow → Red) based on a clock signal.
## Features:
* Two-way intersection control (A and B directions)
* FSM-driven timing for lights:
- Green: 10s
- Yellow: 3s
- Red: Automatically managed by FSM
* Synchronous reset (rst) and clock (clk)
* Easily extendable to include sensors or pedestrian control
## How It Works
The FSM cycles through the following states:
- A Green - B Red
- A Yellow - B Red
- A Red - B Green
- A Red - B Yellow
Each state is held for a specific duration (in clock cycles):
- Green = 10 clock ticks
   Red = 10 clock ticks
- Yellow = 3 clock ticks
## Simulation Output
The simulation waveform confirms that:
- The lights alternate correctly.
- Proper durations for each light are maintained.
- The system resets correctly and resumes normal function.
![image](https://github.com/user-attachments/assets/c2ee1e08-68ed-43ae-a114-d70a7e83f94a)



