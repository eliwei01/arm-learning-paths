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

Each target implementation type might use a different trace capture method. Different trace capture methods might have different functionality, limitations, or usage. For example, to generate and capture trace data, most Arm-based systems use [CoreSight](https://developer.arm.com/Architectures/CoreSight%20Architecture) infrastructure. In contrast, to generate and capture trace events, the Arm [Fixed Virtual Platform (FVP)](https://developer.arm.com/Tools%20and%20Software/Fixed%20Virtual%20Platforms) models use the [Iris](hhttps://developer.arm.com/documentation/101196/latest/?lang=en) API.

During target development, the target could have limitations to the amount or accessibility of the trace infrastructure. Possible limitations might include:

- Inability to capture the same types of trace throughout the target development process 
- Using different trace interfaces, software, or physical connectors

To capture trace data with your target, you might need to adjust your target. The following are possible adjustments necessary to get trace working:

- Work within trace bandwidth restrictions
- Limit the amount of trace data generated
- Adjust trace signals delays
- Modify system clock frequencies

Before tracing, consider the state of your target. For example, tracing your target while it is booting might fail because not all the necessary components are opertional. 

Steps:

1. Determine what type of target implementation you are tracing.
2. Learn about how trace works on your target by consulting your target documentation or designer.
3. Implement the necessary adjustments required to make trace work on your target.
4. Keep up-to-date with changes to your target, these changes can alter or limit your trace capabilities.
5. Consider the target state before tracing.