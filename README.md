# NQubitALU

This is a simple implementation of a simple ALU that allows us to perform addition and substraction for two N-qubit objects.
Implementation in [Qiskit](https://qiskit.org/) was done for scratch for didactic purposes, might not be optimal.

ALU(N) circuit requires a (4N+4) qubit register, where N is the length of the desired qubit strings to operate with.

The registers have to be set in order so that, if you want to add A and B with sub bit SB, and set the result into register S, then the register list has to be of the following order:

[registerA, registerB, registerS, registerSB, registerCarry, registerAncilla]

All registers are of length N, except for register SB which is length 1 and register Ancilla which is length 3.

## Example

After installing qiskit, just run NQubitALU.py from a terminal to see an example.

In the example, I define two 2-bit strings, and simultaneously SUM and SUB the desired strings by setting the SB bit into a Hadamard superposition.

## Other implementations

After writing the code I started researching into other implementations.
Check the following:
https://arxiv.org/abs/1107.3924
