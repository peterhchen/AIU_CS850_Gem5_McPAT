Topics:
1. Gem5 Memory System: Gem5 Memory controller and Gem5 Memory interface 
2. Gem5 Memory Controller
3. gem5 Memory Interface
4. Run example of Linear/Random generator and read/write percentage (50%  or 100%): 
> gem5.opt run-mem.py -c LinearGenerator -r 50
> gem5.opt run-mem.py -c RandomGenerator -r 100
5. Check the m5out/stats.txt: Memory Bandwidth/throughput
6. Simulation result: Multi-channel memory bandwidth is much higher than Single Channel Memory.
