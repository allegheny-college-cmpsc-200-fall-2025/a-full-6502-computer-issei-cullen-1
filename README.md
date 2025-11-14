[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/jL1TaN0Q)
[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/uOmAvT4j)
![Vector art of 200 in hex, subtitle of course: Bare Metal in pale green and printer's black](https://raw.githubusercontent.com/allegheny-college-cmpsc-200-fall-2024/course-materials/media/images/CMPSC%20-%200xC8%20Banner.png)

# ROM-Based 6502 Assembly

| Date              |           |
|:------------------|:----------|
| 7 November 2025   | Assigned  |
| 14 November 2025  | Due       |
| Fundamental            | [![Assignment Progress](../../actions/workflows/main.yml/badge.svg?branch=main)](../../actions/workflows/main.yml) |
| Hack                   | [![Assignment Progress](../../actions/workflows/hack.yml/badge.svg?branch=hack)](../../actions/workflows/hack.yml) |

## Introduction

Your goal for this lab is to finish the build of our 6502-based computers. Here, you have two options to complete the task:

* a `FUNDAMENTAL` which finishes integrating the `6522`
* a `HACK` which adds RAM to your PC using the `62252` SRAM module

Each branch features a test program that proves your setup.

|Branch |Test ROM|
|:------|:-------|
|`FUNDAMENTAL`|[6522 Interface Test](https://github.com/bare-metal-edu/6522-interface-test)|
|`HACK`|[62252 SRAM Test](https://github.com/bare-metal-edu/62256-SRAM-test)

These repositories provide the source as well as the compiled ROMs (also included in the [course schedule](https://chompe.rs/200-schedule).

## Instructions

You must complete and demonstrate this program to an instructor or TL using your breadboard and associated parts. This 
can be done any time during the duration of the assignment until the due date. 

In addition, you must record your findings in the `report.md` file in the `docs/` directory. This documentation will require you to fill
in some truth tables, provide some breadboard layouts, and explain how each of the circuits work, ostensibly. The report also contains
a table for the instructor or TL to fill out when programs are demonstrated. Again, this table _must be filled out by the instructor
or a course TL_. (This means that you'll have to have `commit`s authored by one of these folks!)

## Assignment "Hack"

This assignment's `HACK` asks you to wire the `62252` SRAM chip in order to gain access to writeable memory (SRAM) using the test
program to evidence that your `6502` setup is complete.
