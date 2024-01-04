---
title: What tools to use
weight: 6

### FIXED, DO NOT MODIFY
layout: learningpathall
---

## What tools to use
Many trace tools are available for Arm-based systems. The following are some of the tools available:

- [Arm Development Studio (Arm DS)](https://developer.arm.com/Tools%20and%20Software/Arm%20Development%20Studio) is an Arm created external trace tool that can capture trace from FVP and Arm core-based targets running bare-metal and Linux kernel environments. Arm Development Studio can also decode trace data you have taken from the target manually.
  - To trace hardware targets with Arm Development Studio, you must have a debug probe that supports trace capture like a [DSTREAM debug probe](https://developer.arm.com/Tools%20and%20Software/#q=DSTREAM&aq=%40navigationhierarchiescategories%3D%3D%22Tools%20and%20Software%20products%22%20AND%20%40navigationhierarchiescontenttype%3D%3D%22Product%20Information%22&numberOfResults=48).
  - Read more about tracing with Arm Development Studio and DSTREAM from:
    - <placeholder for new trace document>
    - [Help with debugging and tracing targets guide](https://developer.arm.com/documentation/107551/latest/?lang=en)
    - [Arm Development Studio User Guide](https://developer.arm.com/documentation/101470/latest/?lang=en) 
    - Guide for your debug probe. For DSTREAM, read the appropriate Getting Started Guide and System and Interface Design Reference Guide.
- [OpenCSD](https://github.com/Linaro/OpenCSD) is an Arm created open source tool for external trace.
  - Read more about OpenCSD from:
    - [Is it possible to decode the CoreSight raw trace data offline?](https://developer.arm.com/documentation/ka004902/latest/?lang=en)
    - [Scripts to decode ETE trace stored to a TRBE](https://developer.arm.com/documentation/ka005450/latest/?lang=en)
- [CoreSight Access Library](https://github.com/ARM-software/CSAL) is an Arm created open source tool for performing self-hosted trace in a Linux environment.
- Your company might have its own in-house trace tools that work well with your target or your tracing requirements.

To find the best solution for you, consult colleagues or others knowledgeable in trace.

{{% notice Tip %}}
External trace tools often do not interact well with self-hosted trace. Use external trace or self-hosted trace, not both at the same time.
{{% /notice %}}

Steps:
1. Determine which tools best fit your run environment.
2. If you choose to use a trace tool, learn about its trace capabilities by reading the documentation for the tool.




