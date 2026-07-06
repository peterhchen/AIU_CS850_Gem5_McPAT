Topics:
We discuss the Cache Hierarchy with CHI (Coherence Hub Interface) protocol. CHI is created by ARM. Gem5 maintains the CHI. 
In Full System Simulation, we use a simple traffic generator to generate the traffic and set up the Chi Protocol with Gem5 Standard Library
1. Introduction of AMBA/CHI (Advanced Microcontroller Bus Architecture/Coherence Hub Interface)) Protocol.
2. Create a simple 2-level cache hierarchy by CHI (Coherence Hub Interface) based on ARM SOC (System on Chip).
3. Build 2-level cache hierarchy with Level 1 cache is private to CPU Core and Level 2 cache is a shared directory to a cluster among specific Intel CPU cores. In this example, we do not have L3 to share across all cores.
4. Create Cache Hierarchy, Pass parameter.
5. Create DMA controller
6. Connect the Controller Network.
7. Create Run Script
