---
title: Know your target
weight: 2

### FIXED, DO NOT MODIFY
layout: learningpathall
---

## Know your target
Trace is the process of capturing data that shows how the components in a design are operating, executing, or performing.

The target implementation determines the kinds of trace you can use.

Before tracing your target, you must know what type of target implementation you are using. The following are some examples of target implementation types:

- Simulation
- Emulation
- Software model
- Field Programmable Gate Array (FPGA)
- Development platform
- Production silicon

Each target implementation type might use a different trace capture method. Different trace capture methods might have different functionality, limitations, or usage. For example, to generate and capture trace data, most Arm-based systems use [CoreSight](https://developer.arm.com/Architectures/CoreSight%20Architecture) infrastructure. In contrast, to generate and capture trace events, the Arm [Fixed Virtual Platform](https://developer.arm.com/Tools%20and%20Software/Fixed%20Virtual%20Platforms) models use the [Iris](hhttps://developer.arm.com/documentation/101196/latest/?lang=en) API.

During target development, the target could have limitations to the amount or accessibility of the trace infrastructure. Possible limitations might include:

- Inability to capture the same types of trace throughout the target development process 
- Using different trace interfaces, software, or physical connectors

Due to the target implemention, to capture trace data, adjustments to the target might be necessary. The following are possible adjustments necessary to get trace working:

- Abide by trace bandwidth restrictions
- Limit the amount of trace data generated
- Adjust trace signals delays
- Modify system clock frequencies

Steps:

1. Determine what type of target implementation you are tracing.
2. To learn about tracing your target, consult your target documentation or designer.
3. To make trace work on your target, implement the necessary adjustments.
4. Be aware of any changes to your target that alter or limit your trace capability.