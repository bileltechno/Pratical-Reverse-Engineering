# x86 and x64

The x86 is little-endian architecture, x86 is the 32-bit implementation of the Intel architecture\(IA-32\) as defi ned in the Intel Software Development Manual. Generally speaking,

it can operate in two modes: real and protected. Real mode is the processor state

when it is fi rst powered on and only supports a 16-bit instruction set. Protected

mode is the processor state supporting virtual memory, paging, and other

features; it is the state in which modern operating systems execute. The 64-bit

extension of the architecture is called x64 or x86-64. This chapter discusses the

x86 architecture operating in protected mode.

x86 supports the concept of privilege separation through an abstraction called

ring level. The processor supports four ring levels, numbered from 0 to 3. \(Rings

1 and 2 are not commonly used so they are not discussed here.\) Ring 0 is the

highest privilege level and can modify all system settings. Ring 3 is the lowest

privileged level and can only read/modify a subset of system settings. Hence,

modern operating systems typically implement user/kernel privilege separation

### Register Set and Data Types

### Instruction Set

##### Syntax







