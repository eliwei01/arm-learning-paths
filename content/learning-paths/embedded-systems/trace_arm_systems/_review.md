---
review:
    - questions:
        question: >
            If an Arm processor is tracing another Arm processor on the same chip, what trace mode is used?
        answers:
            - external trace
            - Self-hosted trace
        correct_answer: 1                    
        explanation: >
            Because the processor being traced is not in the same software stack as the processor doing the tracing, the trace mode used is external trace.

    - questions:
        question: >
            If you want to see what instructions were executed by an Armv9-A processor, which trace component do you use?
        answers:
            - ETM
            - ITM
            - ETE
            - STM
        correct_answer: 3                   
        explanation: >
            Armv9-A processor use an ETE to trace instruction execution.



# ================================================================================
#       FIXED, DO NOT MODIFY
# ================================================================================
title: "Review"                 # Always the same title
weight: 20                      # Set to always be larger than the content in this path
layout: "learningpathall"       # All files under learning paths have this same wrapper
---
