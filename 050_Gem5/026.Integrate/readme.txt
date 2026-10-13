gem5/SST Topics: 
gem5 is an useful simulator but not the best for all cases. There are lots of other simulators as well. Gem5 can integrate other simulators, such as, SST, DRAM, etc.
1. core: 
  a. gem5 is small group of cores; SST is highly parallel, multi-scale, 
  b. gem5 in single process in one node. SST in different nodes
  c. gem5 look into one chip. SST across different system.
2. gem5 is a library component of SST.
3. Build/Install gem5 component  
4. SST and gem5 communication
5. SST and gem5 example.
6. To reduce the synchronization cost, we split the simulation by node (machine). Each node gets its own partition (process).
  a. We have multiple nodes (machines), Each node (machine) runs one gem5 component.
  b. In multi-nodes, each machine has 4 cores (CPUs). Each gem5 component runs in a different partition (on different machines)
  c. The gem5 components on different nodes communicate via a PIO device. SST transfers the message to the other node. 
Note: 
  a. A node is a machine, a core is a CPU inside the node (machine). 
  b. Cores do not talk via PIO (Programmed Input/Output). Nodes (machines) talk via PIO.
