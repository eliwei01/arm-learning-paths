---
title: What tools to use
weight: 3

### FIXED, DO NOT MODIFY
layout: learningpathall
---

## What tools to use
The external trace solution you can purchase from Arm is [Arm Development Studio (Arm DS)](https://developer.arm.com/Tools%20and%20Software/Arm%20Development%20Studio). Arm DS can capture trace data from running bare-metal and Linux kernel environments. It can also decode trace data you have taken from the target manually. 

To capture trace with Arm DS, you must have a [DSTREAM debug probe](https://developer.arm.com/Tools%20and%20Software/#q=DSTREAM&aq=%40navigationhierarchiescategories%3D%3D%22Tools%20and%20Software%20products%22%20AND%20%40navigationhierarchiescontenttype%3D%3D%22Product%20Information%22&numberOfResults=48).

Read more about tracing with Arm DS and DSTREAM from:
- <placeholder for new trace document>
- [Help with debugging and tracing targets guide](https://developer.arm.com/documentation/107551/latest/?lang=en)
- [Arm Development Studio User Guide](https://developer.arm.com/documentation/101470/latest/?lang=en)
- Getting Started Guide and System and Interface Design Reference Guide for the DSTREAM you are using

An Arm created, open source solution for external trace is [OpenCSD](https://github.com/Linaro/OpenCSD). See the previous link for more details about OpenCSD.

Many other trace tools and solutions are available for Arm-based systems. For example, your company might have its own in-house trace tools that works well with your target or your tracing requirements. Consult colleagues or others knowledgeable in trace to find the best solution for you.

{{% notice Tip %}}
External trace tools often do not interact well with Self-hosted trace. It is best to use external trace or Self-hosted trace, not both at the same time.
{{% /notice %}}

Steps:
1. Determine which tools best fits your run environment.
2. If you choose to use a trace tool, read the documentation for the tool to learn about its trace capabilities.




