1. How to use CPU Model: AtomicSimpleCPU, TimingSimpleCPU, O3CPU, MinorCPU, and KvmCPU.
2. Setup a simple system with 2 cache size and 3 CPU models.
3. Look at Gem5 generated statistics.
Q. What is difference between the simOps and simInsts?
Ans: a) simInsts: total number of committed instructions. simInsts may contains several simOps. b) simOps: total number of operations, which is a more granular measure than instructions. For RISCV, it is a reduced instruction set. The simInsts and simOps can be very close or the same.
4. Create custom processor based on O3CPU.
5. Big/Little Processors 
