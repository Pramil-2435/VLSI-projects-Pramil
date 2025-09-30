**3-Input Logic Function (Y = (A \* B) + C)**



This repository contains the Hardware Description Language (HDL) implementation and simulation results for a simple 3-input logic function. The design is implemented using Verilog.



**Project Goal**

The primary goal of this project is to implement the following Boolean function:

Y = (A \* B) + C

This function is implemented using a combination of AND and OR gates.



**Design Files**



test1.v: The primary Verilog source code defining the logic function.



schematic diagram.png: The synthesized schematic representation of the design.



waveform.png: The simulation waveform showing the circuit behavior over time.



**Verilog Implementation**

The logic is described structurally using the assign statement in the test1.v module, directly translating the Boolean expression.



test1.v Code Snippet:

module test1(

input a,

input b,

input c,

output y

);



// Implements Y = (A AND B) OR C

assign y = (a \& b) || c;



endmodule



**Circuit Schematic**

The schematic confirms the Verilog code was synthesized into the correct gate-level implementation: an AND gate connected to an OR gate.



**Simulation Results**

The output Y is high (1) when both A and B are high (A AND B), OR whenever C is high.



**Usage and Simulation**

To reproduce the results, you will need a standard HDL simulation tool (e.g., Vivado, ModelSim, or iverilog).



Load the Module: Load the test1.v file.



Create a Testbench: Write a testbench module to apply input stimuli to a, b, and c.





