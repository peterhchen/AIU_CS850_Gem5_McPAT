1. Why Gem5 Standard Library? 
Ans: Standard Library setup the components connection, reduces the redundancy code, predefined components, API to interface the components.
2. What is Gem5 Standard Library?  
Ans: Gem5 Standard Library written in Python and C++. It contains pre-defined  Components, Modular Design, Boards, pre-built systems (X86, ARM, RISC-V, demo system, SiFive Unmatched), Processor, Core.
3. Gem5 create board with Standard Library: 1) Create Memory, 2) Create processor, 3) Create Cache Hierarchy
4. Create X86 Demo Board Code Example:
1) Create Memory (Dual Channel DDR4/2400MHz/4GB, 2) Create processor (Timing Model, X86 ISA, number of core = 2), 3) Create Cache Hierarchy (L1D = 64KB, L1I = 64KB, L2 Size = 8MB. 
5. Create RISC-V Demo Board Code Example:
Ans: 1)  Create Dual Channel DDR4/2400 MHz/4GB), 2) Create processor (Timing Model, RISC-V ISA, number of core = 2, 3) Create cache Hierarch with L1D = 64KB, L1I = 64KB, L2 = 1MB.
6. Create ARM Demo Board Code Example:
1)  Create Dual Channel DDR4/2400MHz/4GB), 2) Create processor (KVM (Kernel-Based Virtual Machine) Model/Timing Model, number of cores =2, ARM ISA , 3) Create cache Hierarch with L1D = 64KB, L1I = 64KB, L2 = 8MB.
