We use compiled Gem5 (Ubuntu in X86) to run cross-compiler (in ARM, AMD, etc) for the Linear Traffic generator and Random Traffic Generator for cache hit/miss rate. 
1. Syscall Emulation Mode: Model the devices of the systems
2. m5ops: gem5 operations
3. How to compile gem5 annotate binary?
a) In the directory bootcamp/materials/02-Using-gem5/03-running-in-gem5/02-annotate-this
b) In the Makefile, we add the compiler GXX = g++, ISA = x86. GEM5_PATH …
c) Change GEM5_PATH to our local gem5, for example
> GEM_PATH = /home/peter/AIU/AIU_CS850_Gem5_McPAT/050_Gem5/gem5
d) Link directory for library search, for example, “-L out/m5”, link all libraries in “out/m5” director.
e) Link specify library, for example, -lm5 means “link libm5 library”
4. Annotate Workloads: 
a) Use workbegin_handler() and workend_handler() for annotation. 
b) Use gem5.opt -re code.py to see the annotation messages.
5. Cross-Compile workloads: We use gem5 (Compiled in X86/Ubuntu) to run other architectures (ARM, AMD, etc)
6. Traffic Generator:
a) Linear Generator simulate the linear memory accesses. Random Generator simulate the random memory accesses.
b) We extend the AbstractGenerator to create the HybridGenerator.
c) We see the difference between the LinearGeneratorCores and RandomGeneratorCores.
