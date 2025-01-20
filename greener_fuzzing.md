---
layout: default
---
# Greener Fuzzing Evaluation 
`For master's or bachelor's thesis`  
   

Fuzzing is a technique of executing and mutating random or semi-random inputs to detect crashing and erroneous behavior in software.
To evaluate improvements in fuzzing, researchers usually use the amount of code covered by a fuzzer as a metric.
This metric is based on the assumption that increased code coverage correlates with a higher likelihood of discovering bugs.
Therefore, to compare fuzzers, they are typically run for 24-hour intervals, with their performance measured by the number of basic blocks covered. Due to the inherent randomness of fuzzing, each fuzzer is run 10 to 20 times on the same sample to ensure the results are statistically significant. Depending on the number of samples, this can require hundreds to thousands of CPU hours, creating a high barrier to entry for new researchers and raising environmental concerns due to the extensive computational resources needed.

Previous research by Lee et al. [[1](https://dl.acm.org/doi/pdf/10.1145/3611643.3616268), [2](https://dl.acm.org/doi/pdf/10.1145/3597503.3639198)] demonstrated that it is possible to estimate the coverage rate of a (greybox) fuzzer. The coverage rate is the probability with which a fuzzer will find new new coverage in a given time frame.
In this work, we want to expand on that, and experimentally test whether it is feasible to replace the standard 24-hour run metric.  
The envisioned metric stops a fuzzer once its coverage rate falls below a certain threshold. This happens when a fuzzer reaches a plateau, where it does not gain any further coverage.
Then, instead of measuring the coverage over 24 hours, we can use the coverage achieved until the fuzzer hits the plateau. 

If this new metric yields results comparable to those from the traditional 24-hour runs, it could significantly shorten the time needed for academic fuzzing evaluations. This would benefit researchers by lowering the entry barrier and reducing the environmental impact associated with large-scale fuzzing experiments.  





