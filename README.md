Fundamentals of Embedded Systems, defines what embedded systems are, howthey are different from other systems, why specific programming techniques are needed,and why C++ is good and in many cases the best choice for embedded development. Itoutlines the constraints and challenges that embedded developers encounter in theireveryday work: limited system resources and CPU performance, dealing with hardwareerrors, and remote debugging

Setting Up the Environment, explains the differences in a developmentenvironment for embedded systems compared to web or desktop application developmentand goes through concepts of the build and target system, cross-compilation and cross-toolkits, the serial console, and the remote shell. It provides practical steps for setting upvirtualized build and target hosts for the most common desktop configurations runningWindows, macOS, or Linux.

Working with Different Architectures, explains how to take into account importantdifferences in CPU architectures and memory configuration of target systems in your C++code.

Handling Interrupts, covers the low-level concepts of interrupts and interruptservice routines. In modern OSes, even developers or device drivers have to use a higher-level API provided by the OS. That is why we explore the interrupt techniques using the8051 microcontroller

Debugging, Logging, and Profiling, covers debugging techniques specific to Linux-based embedded systems, such as running gdb directly on the target board, setting upgdbserver for remote debugging, and the importance of logging for debugging and failureroot cause analysis


Memory Management, provides several recipes and best practices of memoryallocation that will be helpful for developers of embedded systems. We discuss whydynamic memory allocation is avoided in embedded applications and what alternatives canbe considered for fast, deterministic memory allocation

Multithreading and Synchronization, explains how to use the functions and classesprovided by the standard library of C++ to implement efficient multithreading applicationsthat can utilize all the power of the modern multicore CPUs.


Communication and Serialization, covers the concepts, challenges, and bestpractices for inter-process and inter-system communications, such as sockets, pipes, sharedmemory, and memory-efficient serialization using the FlatBuffers library. Decouplingapplications into independent components that talk to each other using well-definedasynchronous protocols is a de facto standard way of scaling a software system whilekeeping it fast and fault-tolerant

Peripherals, explains how to work with various peripheral devices in C++programs. Though most device communication APIs do not depend on a particularprogramming language, we will learn how to use the power of C++ to write wrappers thatare convenient for developers and help prevent common resource leaking errors

Reducing Power Consumption, explores the best practices for writing energy-efficient applications and utilizing the power management functions of the OS. It providesseveral practical recipes for Linux-based embedded systems, but the same concepts can beexpanded to any OS and any platform

Time Points and Intervals, covers various topics related to time manipulations,from measuring intervals to adding delays. We will learn about the API provided by thestandard C++ Chrono library and how it can be used efficiently to build portable embeddedapplications

Error Handling and Fault Tolerance, explores possible implementations and bestpractices of error handling for embedded applications written in C++. It explains how to useC++ exceptions efficiently and compares it to alternatives such as traditional error codesand complex return types. It touches on basic fault-tolerance mechanisms such as watchdogtimers and heartbeats.

Guidelines for Real-Time Systems, covers the specifics of real-time systems. Itbriefly describes how real-time systems are defined and what kinds of real-time systemsexist. It contains practical recipes on how to make the behavior of applications moredeterministic, a crucial requirement for real-time systems.

Guidelines for Safety-Critical Systems, explains what safety-critical systems areand how they are different from other embedded systems. It covers developmentmethodologies and tools that are required when working on safety-critical systems, fromfollowing formalized coding guidelines such as MISRA, AUTOSAR, or JSF to using staticcode analysis or formal software validation tools

Microcontroller Programming, outlines basic concepts of writing, compiling, anddebugging C++ code for microcontrollers. We will learn how to set up the developmentenvironment using the widely used Arduino board as an example