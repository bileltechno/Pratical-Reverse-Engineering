# x86 and x64

The x86 is little-endian architecture, x86 is the 32-bit implementation of the Intel architecture\(IA-32\) .It can operate in two modes: **real** and **protected**.

The 64-bit extension of the architecture is called x64 or x86-64.

This chapter discusses the x86 architecture operating in protected mode. x86 supports the concept of privilege separation through an abstraction called ring level.

### Register Set and Data Types

When operating in protected mode, the x86 architecture has eight 32-bit general-purpose registers \(GPRs\): EAX , EBX , ECX , EDX , EDI , ESI , EBP , and ESP . The instruction pointer is stored in the EIP register.

![](http://www.c-jump.com/CIS77/asm_images/gp_registers.jpg)

| **REGISTER** | **PURPOSE** |
| :--- | :--- |
| ECX | Counter in loops |
| ESI | Source in string/memory operations |
| EDI | Destination in string/memory operations |
| EBP | Base frame pointer |
| ESP | Stack pointer |

The **EFLAGS** is a 32-bit register used as a collection of bits representing Boolean values to store the results of operations and the state of the processor. The names of these bits are:

### 

### Instruction Set

##### Syntax



