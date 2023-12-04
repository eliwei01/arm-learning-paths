---
title: Know your run environment
weight: 2

### FIXED, DO NOT MODIFY
layout: learningpathall
---

## Know your run environment
Trace is the process of capturing data that shows how the components in a design are operating, executing, or performing. What kind of trace is possible is dependent on the target you are using.

For example, depending on the capabilities of the target, Arm-based systems can potential get trace data using two different trace modes: Self-hosted trace or external trace. 

Self-hosted trace happens when the agent controlling the trace collection is part of the same software stack as the software being traced.

External trace happens when the agent controlling the trace collection is outside the software stack being traced. For example, having a debugger setup and control trace capture of a target is external trace.

For more information about Self-hosted trace and external trace, read the appropriate section of the Arm Architecture Reference Manual for the processor profile on your target. For example, if your target has an A-profile processor, read the [Arm Architecture Reference Manual for A-profile architecture](https://developer.arm.com/documentation/ddi0487/latest/).

Step:

1. Determine whether Self-hosted trace or external trace best fits your run environment.
2. If Self-hosted trace best fits, create or find the appropriate software to run for your target.
3. If external trace best fits, determine the external trace method or tool that best fits the target you are working with.

IMAGE HERE:
![example image alt-text#center](example-picture.png "Figure 1. Example image caption")
