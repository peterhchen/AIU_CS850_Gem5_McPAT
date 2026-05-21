Topics:
1. What is Port? 
Port is the interface to move data. We have request and response for data movement.
2. What is Packet?
The Packet class encapsulates all the data/information.
3. Gem5 Port: gem5/src/mem/port.hh contains all the gem5 port declaration.
4. In gem5, we have three access modes: Timing, Atomic, and Functional
- a. Timing Mode: Timing mode is the most detailed and realistic mode. 
- b. Atomic Mode: Atomic mode is a fast mode to model the data movement 
- c. Functional Mode: Functional mode is designed for inspection and debugging.
5. Timing Protocol: Smooth response
6. Timing Protocol: Responder is busy
7. Timing Protocol: Others:
- a. Requestor is busy
- b. Requestor and Responder are busy
