Topics:
1. What is full system simulation?
2. Basics of booting up a real system in gem5
3. How to Setup Gem5 Resource for Full System Simulation?
  a. Go to “https://resources.gem5.org/”
  b. Search for “x84 ubuntu22.04 with systemd” (systemd mean system demon”
  c. Get the string name “x86-ubuntu-22.04-boot-with-systemd” and version “1.0.0”
  d. In the folder 
      > bootcamp/materials/02-Using-gem5/07-full-system/X86-fs-kvm-run.py
  e. Modify the below code
      > workload= obtain-resource (“x86-ubuntu-22.04-boot-with-systemd”, resource_version = “1.0,0”)
      > board.set_workload (workload)
   f. Run the Full System sumulation
3. Creating disk images using Packer and QEMU
4. Extending/modifying a gem5 disk image
5. Using m5term to interact with a running system
