# CODETECH-TASK-ONE
- **Name**: M. Diwakar Reddy
- **Company**: CodeTech IT Solutions
- **ID**: CT08DS8281
- **Domain**: VLSI
- **Duration**: September to October 2024
- **Mentor**: Neela Santhosh Kumar

  ## **project overview**
  ## Table of Contents


- [Introduction](#introduction)
- [Logic Gates](#Logic-Gates)
- [Truth Table](#truth-table)
- [Circuit Diagram](#circuit-diagram)
- [Simulation Results](#simulation-results)

  # Logic Gates Implementation in Verilog

This repository contains the Verilog implementation of basic digital logic gates, along with their simulation results using a waveform viewer.


## Introduction

This project implements basic logic gates such as AND, OR, NOT, NAND, NOR, XOR, and XNOR using Verilog. Each gate is simulated, and the results are visualized using a waveform viewer. These gates are fundamental building blocks in digital electronics, and their Verilog implementations serve as an essential exercise for VLSI design.

## Logic Gates

1. **AND Gate**: Outputs `1` only when both inputs are `1`.
2. **OR Gate**: Outputs `1` if at least one input is `1`.
3. **NOT Gate**: Inverts the input (outputs `1` if input is `0` and vice versa).
4. **NAND Gate**: Outputs `0` only when both inputs are `1` (inverse of AND gate).
5. **NOR Gate**: Outputs `0` if at least one input is `1` (inverse of OR gate).
6. **XOR Gate**: Outputs `1` if the inputs are different.
7. **XNOR Gate**: Outputs `1` if the inputs are the same (inverse of XOR gate).
8. 
   ## simulation-results
<div style="text-align: center;">
    <img src = "TASK-1/WhatsApp Image 2024-10-04 at 6.46.50 PM.jpeg" height = 80% width = 80% title = "Process Flow" >
</div>

## Half Adder Implementation in Verilog

This repository contains the Verilog implementation of a Half Adder, a fundamental combinational logic circuit used to add two single-bit binary numbers.

## Table of Contents

- [Introduction](#introduction)
- [Half Adder](#half-adder)
- [Truth Table](#truth-table)
- [Circuit Diagram](#circuit-diagram)
- [Simulation Results](#simulation-results)
  

## Introduction

A Half Adder is a basic digital circuit that computes the addition of two binary digits. It takes two inputs (A and B) and generates two outputs: Sum and Carry. This repository provides the Verilog implementation of the Half Adder along with its testbench and simulation results.

## Half Adder

The Half Adder performs the addition of two single-bit binary numbers and generates:
- **Sum**: The result of the binary addition.
- **Carry**: The carry-out generated if the sum exceeds 1.

### Truth Table

| A | B | Sum (S) | Carry (C) |
|---|---|---------|-----------|
| 0 | 0 |    0    |     0     |
| 0 | 1 |    1    |     0     |
| 1 | 0 |    1    |     0     |
| 1 | 1 |    0    |     1     |

### Circuit Diagram


The circuit is composed of:
- One XOR gate for the Sum.
- One AND gate for the Carry.
- ## simulation-results
<div style="text-align: center;">
    <img src = "TASK-1/WhatsApp Image 2024-10-04 at 6.52.09 PM.jpeg" height = 80% width = 80% title = "Process Flow" >
</div>


# Full Adder Implementation in Verilog

This repository contains the Verilog implementation of a Full Adder, a fundamental combinational logic circuit used to add three single-bit binary numbers.

## Table of Contents

- [Introduction](#introduction)
- [Full Adder](#full-adder)
- [Truth Table](#truth-table)
- [Circuit Diagram](#circuit-diagram)
- [Simulation Results](#simulation-results)


## Introduction

A Full Adder is a basic digital circuit that computes the addition of three binary digits: two significant bits (A and B) and an input carry bit (Cin). It produces two outputs: Sum and Carry. This repository provides the Verilog implementation of the Full Adder along with its testbench and simulation results.

## Full Adder

The Full Adder adds three single-bit binary numbers: **A**, **B**, and **Cin** (Carry-in), and outputs:
- **Sum**: The result of the binary addition.
- **Carry-out**: The carry-out generated if the sum exceeds 1.

### Truth Table

| A | B | Cin | Sum (S) | Cout (Carry-out) |
|---|---|-----|---------|------------------|
| 0 | 0 |  0  |    0    |        0         |
| 0 | 0 |  1  |    1    |        0         |
| 0 | 1 |  0  |    1    |        0         |
| 0 | 1 |  1  |    0    |        1         |
| 1 | 0 |  0  |    1    |        0         |
| 1 | 0 |  1  |    0    |        1         |
| 1 | 1 |  0  |    0    |        1         |
| 1 | 1 |  1  |    1    |        1         |

### Circuit Diagram


The Full Adder circuit is composed of two **Half Adders** and an **OR gate**:
- The first Half Adder adds A and B to generate an intermediate Sum and Carry.
- The second Half Adder adds the intermediate Sum and Cin to generate the final Sum and Carry.
- The two Carry bits are combined using an OR gate to produce the final Carry-out.
- ## simulation-results
<div style="text-align: center;">
    <img src = "TASK-1/WhatsApp Image 2024-10-04 at 6.55.28 PM.jpeg" height = 80% width = 80% title = "Process Flow" >
</div>

# 4x1 Multiplexer Implementation in Verilog

This repository contains the Verilog implementation of a 4x1 Multiplexer, a fundamental combinational logic circuit used for selecting one of four inputs to pass as output based on control signals.

## Table of Contents

- [Introduction](#introduction)
- [4x1 Multiplexer](#4x1-multiplexer)
- [Truth Table](#truth-table)
- [Circuit Diagram](#circuit-diagram)
- [Simulation Results](#simulation-results)


## Introduction

A **Multiplexer** (or Mux) is a combinational circuit that selects one input from several inputs and forwards it to a single output line. A 4x1 multiplexer selects one out of four inputs based on two select lines (S1 and S0).

## 4x1 Multiplexer

A 4x1 Multiplexer has:
- **4 inputs**: `I0`, `I1`, `I2`, `I3`
- **2 select lines**: `S1`, `S0`
- **1 output**: `Y`

The output `Y` is determined by the combination of select lines, which decides which input (among I0 to I3) will be passed to the output.

### Truth Table

| S1 | S0 | Y (Output) |
|----|----|------------|
|  0 |  0 |     I0     |
|  0 |  1 |     I1     |
|  1 |  0 |     I2     |
|  1 |  1 |     I3     |

### Circuit Diagram



The 4x1 multiplexer uses two select lines to choose between four inputs. Based on the values of S1 and S0, the corresponding input is routed to the output `Y`.
- ## simulation-results
<div style="text-align: center;">
    <img src = "TASK-1/WhatsApp Image 2024-10-04 at 7.02.00 PM.jpeg" height = 80% width = 80% title = "Process Flow" >
</div>



   

