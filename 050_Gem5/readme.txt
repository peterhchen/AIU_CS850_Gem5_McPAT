Open source for computer hardware design: 
a. Before Verilog Implementation: architectural design (Gem5 for cycle-accuracy timing) and McPAT-Calib (Multi-Core Power, Area, Rough Timing)-Machine Learning Calibration/Prediction. 
b. Verilog Implementation: Chisel (FIRRTL) and Spade
We discussed the below topics:
1. What is Gem5 and Gem5 history?
Gem5 = Gems (U. of Wisconsin) for Core simulator + M5 (U. of Michigan) for memory system 
2. Perspective of Computer Architecture Simulation
Core (CPU/GPU), Cache, Network, memory, etc.  
3. Gem5 Software Architecture
- Event Queue driven runs on Virtual Machine
- Python Interface and C++ inheritance BaseCPU Model
