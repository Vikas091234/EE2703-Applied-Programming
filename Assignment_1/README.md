# Assignment 1 – Introduction to Python

## Course

EE2703 – Applied Programming Lab

## Objective

This assignment introduces Python programming through the processing
of SPICE circuit netlist files.

The program reads a circuit description from a netlist file, extracts
the circuit definition between the `.circuit` and `.end` markers,
parses the circuit elements, and prints the circuit elements in
reverse order.

## Learning Outcomes

After completing this assignment, I learned to:

- Read and process text files in Python
- Work with strings and lists
- Split and process lines of text
- Parse structured data from a file
- Use conditional statements and loops
- Handle command-line arguments
- Implement basic error handling
- Work with SPICE netlist files

## Files

| File | Description |
|------|-------------|
| `code.py` | Python program that reads and processes a SPICE netlist. |
| `ckt1.netlist` | Sample SPICE circuit netlist used as input. |
| `ckt2.netlist` | Sample SPICE circuit netlist used as input. |
| `ckt3.netlist` | Sample SPICE circuit netlist used as input. |
| `Assignment 1 - Question.pdf` | Original assignment specification. |

## Program Description

The program accepts a SPICE netlist file as a command-line argument.

It:

1. Opens the specified netlist file.
2. Searches for the `.circuit` and `.end` markers.
3. Extracts the circuit definition between these markers.
4. Processes each circuit-element line.
5. Reverses the order of the circuit elements.
6. Prints the processed circuit definition.

## Input

The program expects a SPICE netlist containing:

```text
.circuit
...
.end