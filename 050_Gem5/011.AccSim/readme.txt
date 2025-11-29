Topics:
1. How to get fast ROI (Region of Interest)?
1.1 Fast forward with KVM (Kernel Virtual Machine)
1.2 Restore a checkpoint (We will discussion in later discussion)
2. Address m5ops Annotation in cpp.
This require to install device driver gem5_bridge.ko (sudo insmod gem5_bridge)
3. Use m5_work_begin() and m5_work_end() to make the ROI (Region if Interest)
4. Use KVM (Kernel Virtual Machine) fast forward for ROI in Python.
4.1 We need to enable the virtualization in the BIOS/UEFI for 
gem5 simulator is running with KVM (Kernel-based Virtual Machine). 
It will take 20 to 30 minutes to download the NPB (NASA Parallel Benchmark) software.
5. Checkpoint of Gem5 (We will discuss later.)
6. Summary of KVM and Checkpoint.
