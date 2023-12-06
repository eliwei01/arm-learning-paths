---
title: What tools to use
weight: 6

### FIXED, DO NOT MODIFY
layout: learningpathall
---

## What tools to use
The external trace solution you can purchase from Arm is [Arm Development Studio (Arm DS)](https://developer.arm.com/Tools%20and%20Software/Arm%20Development%20Studio). Arm DS can capture trace data from bare-metal and Linux kernel environments. Arm DS can also decode trace data you have taken from the target manually. 

To capture trace with Arm DS, you must have a [DSTREAM debug probe](https://developer.arm.com/Tools%20and%20Software/#q=DSTREAM&aq=%40navigationhierarchiescategories%3D%3D%22Tools%20and%20Software%20products%22%20AND%20%40navigationhierarchiescontenttype%3D%3D%22Product%20Information%22&numberOfResults=48).

Read more about tracing with Arm DS and DSTREAM from:

- <placeholder for new trace document>
- [Help with debugging and tracing targets guide](https://developer.arm.com/documentation/107551/latest/?lang=en)
- [Arm Development Studio User Guide](https://developer.arm.com/documentation/101470/latest/?lang=en)
- Getting Started Guide and System and Interface Design Reference Guide for the DSTREAM you are using

If you are looking for an Arm created open source solution for external trace, you might want to consider [OpenCSD](https://github.com/Linaro/OpenCSD).

If tracing in a Linux environment, you might want to consider the Arm created open source solution [CoreSight Access Library](https://github.com/ARM-software/CSAL).

Many other trace tools and solutions are available for Arm-based systems. For example, your company might have its own in-house trace tools that works well with your target or your tracing requirements. To find the best solution for you, consult colleagues or others knowledgeable in trace.

{{% notice Tip %}}
External trace tools often do not interact well with Self-hosted trace. Use external trace or Self-hosted trace, not both at the same time.
{{% /notice %}}

Steps:
1. Determine which tools best fits your run environment.
2. If you choose to use a trace tool, learn about its trace capabilities by reading the documentation for the tool.




