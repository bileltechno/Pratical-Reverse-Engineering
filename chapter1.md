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

![](/assets/Selection_007.png) For more information visit this [link](https://en.wikibooks.org/wiki/X86_Assembly/X86_Architecture#EFLAGS_Register).

The **EIP** register contains the address of the **next **instruction to be executed if no branching is done. EIP can only be read through the stack after a`call`instruction.

### Instruction Set

The x86 instruction set allows a high level of flexibility in terms of data movement between registers and memory. The movement can be classified into five general methods:

* Immediate to register
* Register to register
* Immediate to memory
* Register to memory and vice versa
* Memory to memory

> A classical RISC architecture like ARM can only read/write data from/to memory with load/store instructions \( LDR and STR , respectively\);

##### Syntax

Depending on the assembler/disassembler, there are two syntax notations for x86 assembly code, **Intel** and **AT&T.**In practice, Intel notation is the dominant form and is used throughout this book.

##### Data movement



