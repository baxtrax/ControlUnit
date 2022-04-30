# RISC-V Control Unit
Implements a RISC-V based Control Unit that is used alongside a datapath to create a CPU. Not all instruction types and instructions are supported. This module supports most of R, I, S, B, Type Instructions.

## Details
### The Top Level 0 Diagram
A overview diagram of the Control Unit Module and its inputs and outputs.

![alt text](https://github.com/baxtrax/RISCV-Datapath/blob/main/Images/Datapath-Level0.png?raw=true)

All of these inputs and outputs will be connected to a Datapath that will manipulate the data as needed by the instruction specified.

### Testbench and verification
The Datapath Module is composed of one main file, datapath.v. This module has its own respective testbench to verify the code.

#### Testing and Verification
##### Testing ControlUnit Module (The expected result)
A simple program was made to test the instruction decoding
![alt text](https://github.com/baxtrax/RISCV-Datapath/blob/main/Images/Instr.png?raw=true)
##### Testing ControlUnit Module (Result)
![alt text](https://github.com/baxtrax/RISCV-Datapath/blob/main/Images/Loop1.png?raw=true)

The Control Unit Module has a testbench included if you would want to verify these results.

## Running it
You can use these files with any type of simulation software. This project I personally used Quartus Prime and its simulation package that comes with named ModelSim(Now updated to QuestaSim) but any software that can run and simulate verilog code should do just fine as well.
