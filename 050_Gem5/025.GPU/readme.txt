Below topics are summarized from Professor Matthew Sinclair at University Wisconsin
Topics: 
1. Accelerator: GPU is transformed from Graphic Display Accelerator 
2. GPU Threads vs CPU Memory Latency: GPU uses Parallel Threads vs. CPU Caches to handle Memory latency 
3. NVIDIA CUDA/HIP vs. AMD OpenCL: Thread, Warp, Thread Block, and Kerne)l
4. GPGPU Programming Model: GPU offload the CPU in different phase (kernel). 
5. GPU Hardware: GPU, Shared L2 Cache; Thread/SIMT runs inside Core with private L1 Cache, register, and DDR/HBM memory.  
6. Address Coalescing vs. divergence: We want thread hit memory continuously (coalescing), we do not want divergence (memory segment discontinuously).
7. SIMT (Single Instruction, Multiple thread) Pipeline
8. AMD Matrix Core Engines vs. NVIDIA TensorCores 
9. Memory system optimization: CPU optimize latency, GPU Optimize throughput.
10. CPU Cache vs. GPU Cache: CPU Cache latency reduction. GPU Cache bandwidth filtering (Prevent redundant DRAM traffic). 
11. APU (Accelerated Process Unit, CPU + GPU in one chip) vs. dGPU (Discrete GPU, separated graphics card)
12. gem5 only support AMD GPU: AMD ROCm (Radeon Open Compute) Stack 
13. gem5 has SE (Syscall Emulation) mode simulation and FS (Full System) Mode Simulation. In GPU simulation, gem5 only fully supports FS mode.
14. gem5 simulator is too complicated, gem5 recommends users to use the docker version (download from docker hub)  instead of compiling on your own.
15. checkpoint/restoration: Since gem5 simulation may take a long time (e.g., PyTorch Machine learning training, takes several days or longer). gem5  users can put the checkpoint after the workloads (setup time for kernel, parameters configuration for cache/memory, etc.). 
We want to do the workloads once. Then, we skip the checkpoint/restore the configuration and start simulation after the restoration to the same run time. 
16. Run PyTorch FS Mode
17. Run PyTorch example of MNIST (Modified National Institute Standards and Technology) dataset.
18. Run nanoGPT (Smaller chatGPT) Example.
