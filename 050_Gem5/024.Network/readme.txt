In gem5, Ruby and Garnet are two different components to simulate complex computer system memories and data pathways. Ruby specifies how processors communicate (rules of roads). Garnet is NoC (Network On Chip) Interconnect Model (detailed physical highway, lanes, traffic lights).
Topics:
1. Review Ruby: CPU, L1, L2, Memory, Router, External Link, Internal Lin.
2. NoC (Network on Chip): Garnet can model 3D Vias in Silicon.
3. Create Components: Controller, Router, External Link, Internal Link.
4. Create Ring Topology for CHI Protocol
5. Create Topology File: ring.py,
  a. class Ring,
  b. main Function connectController(),
  c. Specify Core/Cache/Memory components.
  d. Create Router: L1 Cache
  e. Create Link: L2 Cache/Memory
  f. Create External Link: DMA
  g. Create Internal Link
6. Simple Network Structure
7. Create Ring Topology for Ruby Network
8. Create Garnet
