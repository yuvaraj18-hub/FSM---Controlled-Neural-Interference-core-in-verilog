# FSM-Controlled Neural Interference core in Verilog

This project presents a Finite State Machine (FSM)-based controller designed to detect and manage neural interference signals using Verilog HDL. It simulates a digital core capable of handling interference events efficiently, making it suitable for low-power edge computing and neural signal processing applications.

Project Description :

The FSM controls a neural core module by transitioning between states based on input signals that simulate neural interference patterns. This design demonstrates how FSM logic can be used in noise filtering, signal gating, and reactive processing in neuromorphic systems.

Technologies Used :

Verilog HDL – Hardware Description Language for digital design
Testbench – To verify FSM logic with various input cases
GTKWave – To visualize waveform outputs
EDA Playground / ModelSim– For simulation

FSM Working Principle :

The FSM detects interference levels and transitions between different operational states:

IDLE– Waiting for signal
SENSE – Monitoring signal for interference
FILTER – Noise filtering state
RESPOND – Trigger system response
RESET – Return to idle after processing
This structure allows for robust handling of noise or disturbance in digital/neurological signal paths.

 How to Simulate :

 Option 1: Using [EDA Playground](https://edaplayground.com)

1. Go to [EDA Playground](https://www.edaplayground.com/)
2. Paste your `VERILOG.CODE` into the left panel
3. Paste your `TESTBENCH CODE` into the right panel
4. Choose a simulator (e.g., Icarus Verilog)
5. Click Run
6. View the results using GTKWave

Option 2: Local Simulation

1. Use any Verilog simulator like ModelSim or Icarus Verilog:
iverilog -o fsm.vvp VERILOG.CODE TESTBENCH CODE
vvp fsm.vvp
gtkwave dump.vcd
