---
title: Know your target
weight: 2

### FIXED, DO NOT MODIFY
layout: learningpathall
---

## Know your target
Trace is the process of capturing data that shows how the components in a design are operating, executing, or performing.

What kind of trace is possible is dependent on the target you are using.

Before tracing your target, you must know what type of target you are using. Some examples of target types are simulation, emulation, software model, Field Programmable Gate Array (FPGA), development platform, or silicon.

Each target types might use different trace capture methods. Different trace capture methods might have different functionality, limitations, or usage. For example, to generate and capture trace data, most Arm-based systems use [CoreSight](https://developer.arm.com/Architectures/CoreSight%20Architecture) infrastructure. In contrast, to generate and capture of trace events, the Arm [Fixed Virtual Platform](https://developer.arm.com/Tools%20and%20Software/Fixed%20Virtual%20Platforms) models use a [Model Trace Interface (MTI)](https://developer.arm.com/documentation/107925/latest/Introduction-to-trace-components?lang=en).

During target development, the target might have limitations to the amount or accessibility of the trace infrastructure. Some limitations might include:

- Inability to capture the same types of trace throughout the target development process 
- Using different trace interfaces, software, or physical connectors

Due to the target implemention, to capture trace data, adjustments to the target might be necessary. The following are possible adjustments necessary to get trace working:

- Abide by trace bandwidth restrictions
- Limit the amount of trace data generated
- Adjust trace signals delays
- Modify system clock frequencies

Steps:

1. Determine what type of target you are tracing.
2. To learn about tracing your target, consult the target designer or read the target documentation.
3. To make trace work on your target, implement the necessary adjustments.
4. Be aware of any changes to your target that alter or limit your trace capability.