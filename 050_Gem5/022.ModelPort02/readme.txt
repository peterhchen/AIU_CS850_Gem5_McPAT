Topics:
1. Review CPU/Memory Model
2. InspectorGadget (Model CPU/Memory Model):
2.1 Create the inspection buffer.
2.2 Send inspection buffer through the memory side port to the memory.
2.3 Make a request
2.4 Get the responses
2.5 Forward the responses back.
3. Coding (only step 1):
inspector_gadget.hh: Inspector Gadget declaration
inspector_gadget.cc: Inspector Gadget definition
InspectorGadget.py: Top level Python program for user message 
SConscript: Manage Python (InspectorGadget,py), C++ (inspector_gadget.cc), and DebugFlag (user debug command)
4. Four Operations: Receive Functional (Primary function for CPU to Memory), Receive Atomic (Basic Simulator Mode), Receive Timing Request (Accurate Timing), Process Next Request Event (Process Event Queue).
5. Compilation: > scons build/NULL/gem5.opt -j8
