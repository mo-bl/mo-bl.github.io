---
layout: default
---

# Fuzzing firmware with snapshots from real hardware
`For bachelor's thesis`  
  
Emulating and fuzzing firmware can be hard due to different challenges. 
Often tools struggle to get even get the firmware in a state, where it can accept interesting input.  
The idea of this thesis is to run first the firmware on hardware, and stop the execution once a interesting point is reached in order to create a snapshot of the entire device.
Afterward, this snapshot can be loaded into and emulator to serve as the base for fuzzing, as the firmware already is in a booted state.  

This may even allow for more sophisticated fuzzing as we can maybe even mutate the input in the buffers handed to functions.

