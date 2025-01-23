---
title: "Python Basics"
date: "2025-01-24 00:00:00 +0800"
categories: [Python]
tags: [code]
---

# Intel Compiler 8086 Assembly
From my experience, the Intel 8086 Assembly Language is a powerful and low-level programming language that gives you direct control over the CPU and hardware. It’s fascinating because it works so close to the processor itself, which helps you understand how computers really operate at their core.

When I started learning 8086 assembly, I quickly realized that it’s based on the 16-bit architecture of the 8086 processor. This means it can handle operations on 16-bit chunks of data, but it’s also capable of working with 8-bit data when needed. It uses a combination of registers, instructions, and memory addressing to perform tasks.

# Registers in the 8086
One of the first things I learned was how to work with the registers. These are small storage areas inside the processor that play a key role in computations and memory management. Here are the main ones I’ve used:

# General-purpose registers:
These are versatile and used for a variety of tasks:

AX: The accumulator, which is great for arithmetic and I/O operations.
BX: Often used for holding base addresses in memory.
CX: Acts as a counter in loops and shift operations.
DX: Handy for multiplication, division, or working with I/O ports.
# Segment registers:
These are crucial for managing the segmented memory model, which I found unique to the 8086. For example:

CS: Points to the segment of memory where the executable code resides.
DS: Used for the segment holding data.
SS: Manages the stack segment.
ES: Used for extra data storage or string operations.
Other registers like SP (Stack Pointer), BP (Base Pointer), SI (Source Index), and DI (Destination Index) were also interesting because they made working with memory and strings more efficient.

# Instructions and Addressing Modes
What really stood out to me was how many instructions the 8086 provides, and how flexible its addressing modes are. You can use instructions like MOV, ADD, SUB, JMP, and more to manipulate data or control the program flow.

* For addressing, I’ve used:

Immediate Addressing: The data is part of the instruction itself, like MOV AX, 10.
Register Addressing: The data is in a register, e.g., MOV AX, BX.
Direct and Indirect Addressing: These are great for accessing memory directly or via pointers.
My Experience with Writing Programs
One of the first programs I wrote was to print a string using DOS interrupts. It helped me understand how the 8086 interacts with the operating system. Here’s an example I worked on:

```asm
; Program to display "Hello, World!" on the screen

section .data
    msg db 'Hello, World!', '$'  ; String to display (DOS uses $ as the terminator)

section .text
    mov ah, 09h                  ; DOS function to display a string
    lea dx, msg                  ; Load the address of the string into DX
    int 21h                      ; Call interrupt 21h to display the string

    mov ah, 4Ch                  ; DOS function to terminate the program
    int 21h                      ; Call interrupt 21h to exit
```
This program might look simple, but it taught me how to:

Use interrupts (like INT 21h) to interact with the operating system.
Work with data segments and pointers.
Think like the processor does, step by step.
Memory Segmentation and the Stack
One of the challenging but interesting parts of 8086 assembly is the segmented memory model. At first, it felt a bit confusing to manage memory using segments, but once I understood how the segment registers (like CS, DS, and SS) worked together with offsets, it made sense. For instance, the stack uses the SS segment, and I learned to use instructions like PUSH and POP to save and retrieve data efficiently.

# Tools I’ve Used
To practice and test my code, I’ve relied on:

Yjdoc2 : a good intel 8086 compiler with very detailed instructions and guides, although missing a few features and some things are not supported, such as recursive code while using MACROS
