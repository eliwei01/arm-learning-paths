---
title: Which trace to choose
weight: 3

### FIXED, DO NOT MODIFY
layout: learningpathall
---

## Which trace to choose
More recent Arm-based systems implement [CoreSight](https://developer.arm.com/Architectures/CoreSight%20Architecture). CoreSight infrastructure allows trace data to be generated, stored, and moved off-target for analysis. What CoreSight infrastructure a target has is dependent on the target design. 

The following table lists:
- The types of trace you can capture in an Arm-based system.
- A description for each trace type.
- What CoreSight trace component generate the trace type.
 

| Trace type | Description | Associated CoreSight component |
| :---: | :---: | :---: |
| Instruction |  Generate information about the instruction execution of a core or processor | Embedded Trace Extension (ETE) and Embedded Trace Macrocell (ETM) |
| Data |  Generate information about the data accesses of a core or processor | If supported, Embedded Trace Macrocell (ETM). |
| Instrumentation |  Output Operating System (OS) and application events and system information | Instrumentation Trace Macrocell (ITM) |
| System |  Output data about components across the system | System Trace Macrocell (STM) |
| Embedded Logic Analyzer | Capture signal information based on a set of conditions | Embedded Logic Analyzer-600 (ELA-600) and Embedded Logic Analyzer-500 (ELA-500) |
| Coherent mesh network | Capture messages between components in high-end networking and enterprise compute | Coherent Mesh Network (CMN) |

Steps:

1. To determine what CoreSight components are present on the target, consult your target documentation or designer.
2. Based on the CoreSight components implemented and what you are trying to trace, choose the appropriate trace components.

The following are resources on this subject:

- [Learn the architecture - Understanding trace](https://developer.arm.com/documentation/102119/latest/?lang=en)
    - This guide focuses on a high-level view of trace in Armv7 systems, and Armv8 systems up to version Armv8.4.
- [Learn the architecture - Understanding Armv9-A trace guide](https://developer.arm.com/documentation/102856/latest/?lang=en)
    - This guide focuses on the Embedded Trace Extension (ETE) and the Trace Buffer Extension (TRBE) introduced in Armv9-A.
