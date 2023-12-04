---
title: What trace is used for
weight: 4

### FIXED, DO NOT MODIFY
layout: learningpathall
---

## What trace is used for
Trace is often used to diagnose run-time issues or to measure the performance of code.

The following lists the type of trace available and what they could be used for. This list is not exhaustive.

- Instruction
  - Diagnosing execution issues like code executing when it should not or executing in the wrong place.
  - If cycle counting or timestamping is enabled, measuring the performance or timing of executed code.
  - If timestamping is enabled, corrolating activities across multiple components on the target.
- Data
  - Diagnosing execution issues like code using the wrong data or the correct data not being accessed. 
- Instrumentation
  - Outputting printf-style debugging.
  - On a Cortex-M processor, dumping useful core information.
- System
  - Monitoring signals outside the processor to show a wider scope of target activity.
- Embedded Logic Analyzer
  - Diagnosing target issues at the signal-level. 
- Coherent mesh network
  - Captures messages between components attached to the CMN.

Steps:
- Based on the issue you are experiencing or the performance you wish to measure, choose the appropriate type of trace to use.
- Setup the necessary CoreSight components on the target to capture the trace data you are looking for. Perform this setup either manually, with code, or with a tool. 

