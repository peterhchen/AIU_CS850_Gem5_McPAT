Gem5 core simulator is shingle thread. Multi-thread share code, data, and heap memory. Multi-Process does not share code, data, and heap memory. 
Gem5 Multisim implement multi-processing. Multisim does not implement multi-thread simulation. 
Gem5 Multisim uses script and configuration to produce the consistent output format.
Topics:
1. Gem5 Single thread Problem
2. Gem5 Insight
3. Multi-Processing by Script
4. Multi-Processing by Script vs. Multisim
5. Implement Multi-Processing by Multisim: 
  5.1 Import Multisim, 
  5.2 Setup Number of Processor will be used.
  5.3 Setup Process: CPU Timing Model, ISA type: X86/ARM/AMD, Core  
  5.4 Loop structure of Cache Cache and Instruction Cache
  5.5 Memory Model: DDR3 Channel
  5.6 Setup Board (Clock frequency, Processor, Cache, Memory) 
6. Run Multisim with Single Script
7. Display Multisim Configuration 
