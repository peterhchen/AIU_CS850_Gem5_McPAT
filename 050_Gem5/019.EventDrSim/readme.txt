The gem5 simulator is a discrete event-driven simulator. The time only advances when specific actions, called Events, rather than simulating every clock cycle.
1. Events: Each event is a C++ object that contains a callback function.
2. Scheduling: Events are scheduled to execute at a specific future "tick" (the smallest unit of time in gem5).
3. Execution: The simulator pulls the event with the earliest timestamp from the queue, sets the current simulation time to that event's timestamp, and executes its callback function.
4. Key Simulation Components: SimObjects, EventWrappe, and startup() Phase.
5. Code example 1: SimObject Event
6. Code example 2: SimObject as the passing parameter.
7. Specified the user files in gem5/src/SConscript: Python, C++ header file, C++ source file
8. Compilation: scons gem5/build/NULL/gem5.opt -j8    
    - NULL is used for development without tie to any archecture (X86,ARM, etc).
    - j8 means jobs compiled in 8 cores.
