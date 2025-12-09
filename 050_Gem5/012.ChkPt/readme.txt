Topics:
1. Review of KVM Fast-Forward
2. Gem5 Checkpoint
3. Checkpoint and Restore
4. KVM
4.1 KVM advantage
a. It is fast-forward at nearly the host native speed. 
b. It is flexible to simulation system change
c. It is flexible to workload and software changes.
4.2 KVM disadvantage
a. It is Non-deterministic
b. The host must match the guest ISA (Instruction Set Architecture)
c. Currently, we do not have the RISCV support for KVM.
5. Checkpoint 
5.1 Checkpoint advantage
a. We can create one and run it many times and may different system
b. Almost all devices and components are supported.
5.2 Checkpoint disadvantage
a. It cannot change workload and software at all between the checkpointing and restoring.
b. Checkpoint have restrictions on simulation system changes between checkpoint and restore script.
c. Checkpoint requires disk space.   
