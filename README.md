# Car-Parking-Control-System-Using-VHDL
A VHDL-based car parking system using FSM with sensor input, password verification, LED indicators, and 7-segment display. Simulates entry control and vehicle flow with a testbench and waveform validation in Vivado.

🚗Car Parking System using VHDL and FSM

This project implements a Car Parking System using VHDL based on a Finite State Machine (FSM) architecture. It simulates the behavior of a real-world automated parking gate system, with access control via password input and vehicle detection using front and back sensors.

🔧 Key Features:
FSM-Based Design: Includes states such as IDLE, WAIT_PASSWORD, WRONG_PASS, RIGHT_PASS, and STOP for handling parking logic.

Sensor Input:

Front Sensor: Detects vehicles approaching the gate.

Back Sensor: Confirms vehicle has passed through the gate.

Password Verification:

A 2-part binary password must be entered.

Correct password → Green LED blinks.

Incorrect password → Red LED blinks until correct input.

Visual Indicators:

7-Segment Displays show system state.

LEDs provide visual access feedback (entry granted/denied).

Simulation:

Fully verified using testbench in Vivado or ModelSim.

Includes waveform output for validation.

🛠️ Tools & Technologies:
VHDL (RTL Design)

* Vivado (Simulation & Synthesis)

* ModelSim (Optional Simulation)

* FSM Modeling

* 7-Segment Display Control

* LED Indicator Control

📁 Files Included:
Car_Parking_System_VHDL.vhd – Main VHDL module

tb_car_parking_system_VHDL.vhd – Testbench for simulation

README.md – Project description

Simulation waveforms/video

🚀 How It Works:
System starts in IDLE.

Vehicle detected by front sensor → transitions to WAIT_PASSWORD.

If correct password is entered within 4 clock cycles → RIGHT_PASS (Green LED blinks).

If incorrect → WRONG_PASS (Red LED blinks repeatedly).

Once the car passes through (detected by back sensor), system returns to IDLE or enters STOP if another vehicle arrives.

