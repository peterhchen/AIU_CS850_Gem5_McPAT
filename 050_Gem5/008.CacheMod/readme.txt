Cache hierarchy include L1 [L1I (Instruction Cache) and L1D (Data Cache) in CPU and in Core], L2 (not in CPU, but in Core), L3 (Not in CPU and not in Core, Shared by Multiple CPUs)
1. What is Cache Coherence?
Ans: In Multi-Core, Cache coherence ensures all cores have consistent/up-to-date of shared memory. To prevent multiple, conflict of the same data in different caches, the Cache Coherence protocols are used to resolve the inconsistent data in caches.
2. What do we have Classic Cache and Ruby Cache?
Ans: Gem5 merge M5 (from University of Michigan) and GEMS (from University of Wisconsin). Classic Cache is from M5 and Ruby is from GEMS.
3. What is difference from Classic Cache and Ruby Cache?
Ans: Classic Cache: Original M5 (SimObject) from University of Michigan for simple cache Simulation.
Ruby Cache: provide the flexible Cache Coherence Protocol merged from GEM5 to resolve the Cache Coherence problem.
