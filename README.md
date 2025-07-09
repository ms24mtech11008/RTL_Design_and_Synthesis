# RTL_Design_and_Synthesis
## Table of contents
- [Day 1 - Introduction to Verilog RTL design and Synthesis](#Day-1---Introduction-to-Verilog-RTL-design-and-Synthesis)
 - [Introduction to open-source simulator iverilog](#Introduction-to-open-source-simulator-iverilog)
  - [SKY130RTL D1SK1 L1 Introduction to iverilog design test bench](#SKY130RTL-D1SK1-L1-Introduction-to-iverilog-design-test-bench)




# Day 1 - Introduction to Verilog RTL design and Synthesis
## Introduction to open-source simulator iverilog
---
### SKY130RTL D1SK1 L1 Introduction to iverilog design test bench
---

A **simulator** is a tool used to verify the behavior of a design. In RTL design, the simulator checks whether the design adheres to the specifications by applying a set of input stimuli.

In this course, we are using **Icarus Verilog (iverilog)** as the simulation tool.

### What is a Design?

A **design** is the actual Verilog code or a set of Verilog modules that implement the intended functionality to meet the required specifications.

### What is a Test Bench?

A **test bench** is the setup used to apply input stimuli (test vectors) to the design in order to verify its functionality. It provides the inputs and checks the outputs of the design during simulation.

### How Does a Simulator Work?

The simulator monitors the input signals for any changes.

* When an input changes, the simulator evaluates and updates the outputs accordingly.
* If there is no change in the inputs, the outputs remain unchanged.
  The simulator is event-driven and responds only to input value changes.

### Design and Test Bench Setup

The design contains one or more **primary inputs** and **primary outputs**.
The **test bench** includes:

* A **stimulus generator** to apply input signals to the design.
* A **stimulus observer** to monitor and verify the outputs.

All these components together form the test bench environment.

**Note:** The test bench itself does not have any primary inputs or outputs. It operates entirely within the simulation environment to drive and observe the design.

![Screenshot 2025-07-09 130655](https://github.com/user-attachments/assets/c85f95a3-6840-47e1-9fe2-c673c71d2915)

---

