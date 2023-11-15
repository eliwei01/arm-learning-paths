---
title: Which trace to choose
weight: 3

### FIXED, DO NOT MODIFY
layout: learningpathall
---

## Which trace to choose
More recent Arm-based systems implement [CoreSight](https://developer.arm.com/Architectures/CoreSight%20Architecture). CoreSight infrastructure allows trace data to be generated, stored, or moved off-target for analysis. How and what CoreSight infrastructure a target has is dependent on the target designer.

| Trace type | Description | Associated CoreSight component |
| :---: | :---: | :---: |
| Instruction |  Generates information about the instruction execution of a core or processor | Embedded Trace Extension (ETE) and Embedded Trace Macrocell (ETM) |
| Data |  Generates information about the data accesses of a core or processor | If supported, Embedded Trace Macrocell (ETM) |
| Instrumentation |  Outputs Operating System (OS) and application events and system information | Instrumentation Trace Macrocell (ITM) |
| System |  Outputs data about components across the system | System Trace Macrocell (STM) |
| Embedded Logic Analyzer | Captures signal information based on a set of conditions | Embedded Logic Analyzer-600 (ELA-600) and Embedded Logic Analyzer-500 (ELA-500) |
| Coherent mesh network | Captures messages between components in high-end networking and enterprise compute | Coherent Mesh Network (CMN) |

Steps:

1. Consult your target documentation or designer to determine what CoreSight components are present on the target.
2. Based on what CoreSight components are implemented and what you are trying to trace, choose which trace components to use.

Resources on this subject:

- [Learn the architecture - Understanding trace](https://developer.arm.com/documentation/102119/latest/?lang=en)
    - This guide focuses on a high-level view of trace in Armv7 systems, and Armv8 systems up to version Armv8.4.
- [Learn the architecture - Understanding Armv9-A trace guide](https://developer.arm.com/documentation/102856/latest/?lang=en)
    - This guide focuses on the Embedded Trace Extension (ETE) and the Trace Buffer Extension (TRBE)introduced in Armv9-A.
