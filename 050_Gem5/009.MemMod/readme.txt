Topics:
1. Gem5 Memory System: Gem5 Memory controller and Gem5 Memory interface 
2. Gem5 Memory Controller
3. gem5 Memory Interface
4. Run example of Linear/Random generator and read/write percentage (50%  or 100%): 
> gem5.opt run-mem.py -c LinearGenerator -r 50
> gem5.opt run-mem.py -c RandomGenerator -r 100
5. Check the m5out/stats.txt: Memory Bandwidth/throughput
6. Simulation result: 
  a. The multi channel memory bandwidth is much higher that single channel memory.
  b. Multi-channel memory bandwidth is much higher than Single Channel Memory. 100% read has higher bandwidth than 50% read/write. 
7. Comm Monitor (Communication Monitor) is a very useful tool to check the bandwidth, read byes /write bytes histogram of crossbar and find the bottleneck.
8. In the standard library for memory: ./gem5/src/python/gem5/components/memory/memory.py
Below, we look at how AddrRange() function convert the address into the parallel DRAM channels.
  a. Take log for channel number.
  b. Loop the memory control and use AddrRange() convert the DRAM range.
  c. The AddrRange () convert based on start address, size and interleave low bit, interleave bits, select match channel, etc.
