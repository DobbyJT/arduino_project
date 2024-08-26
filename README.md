# We-the-system

This repository is made for the project 11 team of the Microprocessor Application System Project.

In this project we're using hiwonder ackerman steering with Arduino MEGA.

We'll be doing Regenerative System, PID Control, Wireless Communication, Line Tracing

This code is based on Arduino(C++ language) and will be discussing uses in Project of implementing mechanism of Regenerative system, DC motor’s PID control, Line Tracing

Following paper presents circuit of the regenerative system, with the rectifier and switching calculation.

Vehicle used in the project is RWD with front steering.

Each DC motors will be connected to the batteries and Microprocessor; be charged and powered at same batteries.

PID control will be functioning and show each function for p, i, d.

Since, there are many systems and interrupts, we decided to devide hardware to behave efficiently.

The Arduino_mega_dc is about main motor and it has code about pid for synchronizing two motors and pid for target speed.

The Arduino_uno_regen is code for systme of regenerative braking. Since we use relay module, there should be code with it to divide voltage in and out. 

The Arduino_uno_servo is code for steering and lane tracing. 

We also put our subsystems and trials in subsystem folder. 
