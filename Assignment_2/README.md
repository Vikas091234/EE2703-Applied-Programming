# Assignment 2 – SPICE Part 2

## Course

EE2703 – Applied Programming Lab

## Objective

This assignment extends the SPICE program developed in Assignment 1.
The program parses a SPICE netlist, represents circuit components
using Python classes, constructs the matrix equations for the circuit,
and solves for node voltages and currents.

## Learning Outcomes

After completing this assignment, I learned to:

- Use classes and objects in Python
- Represent circuit components using objects
- Parse different types of SPICE components
- Convert engineering notation into numerical values
- Assign numerical indices to circuit nodes
- Construct matrix equations for circuit analysis
- Use NumPy arrays and matrices
- Solve systems of linear equations using `numpy.linalg.solve()`
- Handle DC and AC circuit sources
- Handle dependent sources
- Process complex-valued circuit quantities

## Files

| File | Description |
|------|-------------|
| `code.py` | Supporting Python examples for the assignment. |
| `code(1).py` | Main SPICE circuit parser and circuit solver. |
| `3.0.1.py` | Python list-unpacking exercise from the assignment material. |
| `4.2.1.py` | NumPy array and indexing exercise from the assignment material. |
| `ckt1.netlist` – `ckt8.netlist` | SPICE circuit input files used for testing. |
| `Assignment 2 - Question.pdf` | Original assignment specification. |

## Program Description

The main program performs the following steps:

1. Reads a SPICE netlist file.
2. Identifies the `.circuit` and `.end` sections.
3. Parses the circuit components.
4. Creates Python objects representing different component types.
5. Converts engineering notation such as `1k`, `1m`, `1u`, and `1n`
   into numerical values.
6. Identifies all circuit nodes.
7. Assigns numerical indices to the nodes.
8. Constructs the matrix equation:

   Mx = b

9. Solves the system using `numpy.linalg.solve()`.
10. Displays the calculated node voltages and source currents.

## Circuit Components

The program supports:

- Resistors
- Capacitors
- Inductors
- Independent voltage sources
- Independent current sources
- Voltage-controlled voltage sources (VCVS)
- Voltage-controlled current sources (VCCS)
- Current-controlled voltage sources (CCVS)
- Current-controlled current sources (CCCS)

## Concepts Used

- Python classes and objects
- Object-oriented programming
- File handling
- String parsing
- Dictionaries
- Lists
- NumPy arrays
- Complex numbers
- Matrix construction
- Linear equation solving
- SPICE netlists
- Modified nodal analysis

## Running the Program

Run the main program with a SPICE netlist:

```bash
python code(1).py ckt1.netlist