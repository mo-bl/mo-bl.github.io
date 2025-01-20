---
layout: default
---
# Directed Firmware Fuzzing
`For master's thesis`

A technique which has been thoroughly explored and is still being actively researched in general-purpose fuzzing is [directed fuzzing](https://github.com/strongcourage/awesome-directed-fuzzing).
The general idea is that we want to target specific areas within the code instead of distributing our attention evenly.
This can be used for regression test, day-1 vulnerability detection, and fuzzing of code areas deemed unsecure through static analysis.  

The general idea of this thesis is that we want to apply directed fuzzing to firmware, to move the execution flow away from undesired aspects of the firmware and towards interesting data processing. To this end we face several challenges:
- Binary nature of firmware makes it harder to apply some analysis techniques
- Firmware does not consume input in a monolithic block but in individual chunks distributed across a vast input file
- ...

As part of this master's thesis you would extend an existing firmware fuzzer to incorporate techniques for directed fuzzing or create your own tool that is specifically designed to solve the problems in this area
