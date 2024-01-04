---
title: What trace is used for
weight: 5

### FIXED, DO NOT MODIFY
layout: learningpathall
---

## What trace is used for
Trace is often used to diagnose run-time issues or to measure code performance.

The following lists the type of trace available and their possible uses. This list is not exhaustive.

- Instruction
  - Diagnosing execution issues like code executing incorrectly or executing in the wrong place.
  - If enabling cycle counting or timestamping, measuring the performance or timing of executed code.
  - If enabling timestamping, correlating activities across multiple components on the target.
- Data
  - Diagnosing execution issues like code using the wrong data or the correct data not being accessed. 
- Instrumentation
  - Outputting printf-style debugging.
  - On a Cortex-M core, dumping useful core information.
- System
  - Show a wider scope of target activity, monitoring signals outside the core.
- Embedded logic analyzer
  - Diagnosing target issues at the signal level. 
- Coherent mesh network
  - Captures messages between components attached to the CMN.

Steps:
- Based on the issue you are experiencing or the performance you want to measure, use the appropriate type of trace.
- Set up the necessary CoreSight components on the target to capture the trace data you want. Perform this setup either manually, with code, or with a tool. 

