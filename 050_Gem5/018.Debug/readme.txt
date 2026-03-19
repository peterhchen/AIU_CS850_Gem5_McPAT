Topics:
1. Debug Flags: Gem5 provides DebugFlags to print the register and memory information for debugging. 
2. SimObject DebugFlags: We add configuration in SConscript, Debug information in python code, C++ header/Code. 
3. In Gem5, we recommend using assertion for run-time logic error checking instead of debugging print.
  - 3.1 panic to catch developer mistakes. 
  - 3.2 fatal to prevent user mistakes.
