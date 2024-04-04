# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

# AIM:

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

# Equipments Required:

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

# Full Adder and Full Subtractor

## Full Adder

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

## Figure -1 FULL ADDER

## Full Subtractor

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

## Truthtable:
![image](https://github.com/arbasil05/FULL_ADDER_SUBTRACTOR/assets/144218037/8556aac6-03ff-4249-b959-6cf8fa5074f2)


The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/arbasil05/FULL_ADDER_SUBTRACTOR/assets/144218037/7a13b0b0-081b-4581-975a-12d91a4f9c8c)



## Procedure:

STEP-1 Define Inputs and Outputs

STEP-2 Understand the Encoder Functionality

STEP-3 Design the Functional Table

STEP-4 Write Verilog Code

STEP-5 Verify Verilog Code

STEP-6 Synthesize the Design

STEP-7 Implement in FPGA

STEP-8 Verify Functionality on FPGA

# Program:

```
module Exp_05(a0,a1,a2,d0,d1,d2,d3,d4,d5,d6,d7);
input d0,d1,d2,d3,d4,d5,d6,d7;
output a0,a1,a2;
assign a0=d1|d3|d5|d7;
assign a1=d2|d3|d6|d7;
assign a2=d4|d5|d6|d7;
endmodule
```

# RTL Schematic:
![image](https://github.com/arbasil05/FULL_ADDER_SUBTRACTOR/assets/144218037/1c730a85-c9bd-4b5a-8cfa-755689b16681)


# Output Timing Waveform:
![image](https://github.com/arbasil05/FULL_ADDER_SUBTRACTOR/assets/144218037/93bc4d8c-e3f8-4864-a5de-d7c05aa9b211)


# Result:

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



