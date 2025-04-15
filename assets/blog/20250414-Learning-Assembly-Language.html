# Learning Assembly Language

Date: April 14th, 2025
Author: Robert Crawford
Tags: Assembly Language, Programming, Low Level

## Introduction

I recently got a new MacBook and I've really been enjoying the experience. However, I've wanted to delve into something new and exciting and just doing some general research has lead me to the following website: https://mariokartwii.com/armv8/ which seems like an extremely approachable and easy to understand resource to learn just that.

I know basic programming and have coded in low level languages such as C using "The C Programming Language" book. I really enjoy programming in C compared to some of the higher level languages and I can't really articulate the reason as to why but it feels like I'm more in control or something.

My current goal is just to learn enough requisite information to write up your typical "Hello, world" program but this time in assembly. I mean, that sounds more important than preparing for the provincial Skills Canada competetion anyways, right?

I'm also going to document some of the key information that I find most important along my journey so perhaps you may find something useful in this disorganized chaos of a "blog post".

## CPU, Binary, and Assembly

A CPU only understands binary but writing an entire program in 1s and 0s would probably be comparable to writing a program in [brainfuck](https://brainfuck.org) (excuse my language - that's what the programming language is called). Therefore, smart people came up with assembly language which is about as low as we can go without driving ourselves mad.

Going one level higher, we have C which is compiled into assembly before it is finally converted into machine code which can be read by a CPU. This is beneficial because we can write a single program in C and then translate it into multiple different assembly languages instead of writing the same program multiple times for different CPUs.

### Then Why Learn Assembly?

Personally, I prefer a bottoms up approach to learning because I find it hard to conceptualize things when I don't have a foundational understanding of the underlying layers. When I'm troubleshooting network issues, I don't start from the application layer - I start from the physical layer and work my way up.

However, the tutorial linked above does present some good alternative reasons for learning assembly:
- Writing out the Boot/Reset Sequence for a CPU
- Writing out CPU-specific specialized tasks
- Performance
- Understanding a specific CPU as much as possible
- Exploits/Hacks for a specific CPU (such as for Video Game Consoles)
- A better understanding of "under the hood" stuff (such as Memory Management, Cache, etc.)

## Definitions

Quoting Gerald Sussman, "in order to have control over a spirit, you must first know the name of that spirit". So, this section is mostly going to be a list of definitions and terms that are probably important to know.

- Binary Numbers (base 2)
- Bits
- Hexadecimal Numbers (base 16)
- 0x (hexadecimal prefix)
- Null (0)
- Byte (8 bits - 1 hex digit)
- Halfword (16 bits - 2 hex digits)
- Word (32 bits - 8 hex digits) 
- Double-Word (64 bits - 16 hex digits)
- Quadword (128 bits - 32 hex digits)

When you have any value length, the left half is known as the "upper" portion and the right half is known as the "lower" portion.

All of ARMv8 AArch64's instructions are 32-bits in length.

## Memory? I forget what that is.

A CPU's instructions reside in RAM and so does any data that the CPU needs to read/write. 

**Static/Main Memory**
The region where a CPU's instructions reside is called Static or Main memory because the same program's instructions will be located in the same location of memory every time it's executed.

**Dynamic/Heap Memory**
The region of memory where data is kept is called Dynamic or Heap memory. The locations of this data is subject to change and may not be in the same location.

**Memory Addresses**
Locations in memory are called memory addresses and are typically a fixed length when referenced by a CPU.

Understanding values located in memory is important. The original article has a really good diagram and explaination of how to do just that so instead of repeating the same information (which I'm basically already doing), I'm just going to link to it [here](https://mariokartwii.com/armv8/ch3.html#:~:text=Understanding%20values%20located%20in%20Memory:).

The author includes a good point which I feel is important to repeat: "If you can visualize it, you can write code for it."

## Registers

Registers are another place where a CPU will keep data at. However, they 
are much smaller and faster than RAM and are at the top of the computer memory heirarchy. 

TODO: Insert a free image of computer memory heirarchy.

There are three main groups of registers:
1. General Purpose Registers (GPRs)
2. Floating Point Registers (FPRs)
3. Special Purpose Registers (SPRs)

Each GPR is 64-bits in length - a double word is the maximum size data type that can fit into a GPR. GPR's can be modified by the CPU and can contain a Memory Address or some basic value.

- r29 is known as the Frame Pointer (FP)
- r30 is known as the Link Register (LR)

The Link Register is used for subroutines within a program and usually contains a memory address.

There's also a register known as the Zero Register which you cannot write to. It always contains the value of zero.

The Program Counter (PC) is a read-only register. It keeps track of the memory address where the CPU is currently executing within a program. The Stack Pointer (SP) is used with the LR for subroutines and will always contain a Memory Address.

## The Fun Part

So... that's been a lot of theory and things to remember but now we are moving on to the hands-on part where we actually get to write some code.

I guess the things that I currently need are an assembler, a linker, and an object dumper to analyze an object file. I know I have the Apple Assembler `as`, the Darwin Linker `ld`, and the Apple LLVM `objdump` so I'm going to try to use those. The original article's author uses Linux so they're using the GCC versions of the aforementioned.

# TODO

- Program a decimal-to-hex / hex-to-decimal converter.
    - Link it here (maybe write it in JS?)
- Make flash cards to memorize terminology.
    - Datatypes and their sizes
    - Registers and their purpose
