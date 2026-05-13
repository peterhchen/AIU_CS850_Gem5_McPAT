Topics:
1. sWhat is ISA (Instruction Set Architecture)?
2. ISA/CPU Independence
3. StaticInst (Static Instruction) and DynInst (Dynamic Instruction): In StaticInst, the architectural definition of an instruction (opcode, operands, behavior) are decoded once and cached and does not change. DynInst contains dynamic information like specific register values, physical register mappings, PC (Program Counter), and prediction information.
4. ExecContext: ExecContext is an abstract base class that defines the interface operation of ISA (Instruction Set Architecture) and CPU model. 
5. ISA (Instruction Set Architecture) Example
6. Memory Access for Instruction Execution
7. ISA (Instruction Set Architecture) Parser
8. RISC-V Instruction Format
9. Exercise: Implement ADD16: Define RISC-V ISA for ADD16, Compile into C++ Code, Run gem5 with new ISA with ADD16.
