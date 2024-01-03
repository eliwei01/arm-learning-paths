---
title: Know your run environment
weight: 3

### FIXED, DO NOT MODIFY
layout: learningpathall
---

## Know your run environment
Depending on the capabilities of the target, Arm-based systems can potentially get trace data using 2 different trace modes: self-hosted trace or external trace. 

Self-hosted trace happens when the agent controlling the trace collection is part of the same software stack as the software being traced.

External trace happens when the agent controlling the trace collection is outside the software stack being traced. For example, having a debugger setup and control trace capture of a target is external trace. An additional example is if a core outside the software stack setups and controls trace capture for another core in the system.  

For more information about self-hosted and external trace, read the appropriate section of the Arm Architecture Reference Manual for the core profile on your target. For example, if your target has an A-profile core, read the [Arm Architecture Reference Manual for A-profile architecture](https://developer.arm.com/documentation/ddi0487/latest/).

Steps:

1. Determine whether self-hosted trace or external trace best fits your run environment.
2. If self-hosted trace best fits, create or run the appropriate software for your target.
3. If external trace best fits, determine the external trace method or tool that best fits the target you are working with.