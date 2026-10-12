gem5/SST Topics: 
gem5 is an useful simulator but not the best for all cases. There are lots of other simulators as well. Gem5 can integrate other simulators, such as, SST, DRAM, etc.
1. gem5 is a library component of SST.
2. Build/Install gem5 component  
3. SST and gem5 communication
4. SST and gem5 example.
5. To reduce the synchronization cost, we split the simulation by node (machine). Each node gets its own partition (process).
5.1. We have multiple nodes (machines), Each node (machine) runs one gem5 component.
5.2. The multi-node setup is a setup for multiple machines. For example, each machine has 4 cores (CPUs). Each gem5 component runs in a different partition (on different machines)
5.3. The gem5 components on different machines communicate via a PIO device.  One node writes a message into PIO registers. SST transfers the message to the other node (machine). 
Note: 
a. A node is a machine, a core is a CPU inside the node (machine). 
b. Cores do not talk via PIO (Programmed Input/Output). Nodes (machines) talk via PIO.
