Embedded Robot Control using AT89C51
📌 Project Overview

This project implements a basic embedded robot control system using the AT89C51 microcontroller.
The robot uses two DC motors driven through a motor driver, and its movement is controlled using five switches.

Each switch press results in a specific movement of the robot such as forward, backward, left, right, or stop.

🎯 Objective

Interface AT89C51 with a motor driver

Control two motors using digital output pins

Use switch-based control for robot movement

Implement simple decision logic using Embedded C

🧰 Hardware Used

AT89C51 Microcontroller

Motor Driver

Two DC Motors

Five Switches

(No additional components are considered beyond what is used in the code.)

⚙️ Software Used

Keil µVision (Embedded C programming)

Proteus (Simulation)

🔌 Pin Configuration (As per Code)
Motor Control Pins (Port 1)
Signal	Pin
Motor 1 Positive (m1p)	P1.0
Motor 1 Negative (m1n)	P1.1
Motor 2 Positive (m2p)	P1.2
Motor 2 Negative (m2n)	P1.3
Switch Inputs (Port 1)
Switch	Pin
Switch 1	P1.0
Switch 2	P1.1
Switch 3	P1.2
Switch 4	P1.3
Switch 5	P1.4
🧠 Working Principle (Derived from Code)

All motor outputs are initially set to LOW

The program runs in an infinite loop

Each switch press is continuously checked

Based on the switch pressed, motor direction is controlled

🚗 Robot Movement Logic
Switch Pressed	Motor Action	Robot Movement
SW1 = 0	Both motors forward	Forward
SW2 = 0	Both motors reverse	Backward
SW3 = 0	Motor 1 reverse, Motor 2 forward	Left
SW4 = 0	Motor 1 forward, Motor 2 reverse	Right
SW5 = 0	Both motors stop	Stop
