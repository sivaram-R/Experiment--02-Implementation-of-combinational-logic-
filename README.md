# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.

 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output. F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

1.AND gate The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB Y= A.B

2.OR gate The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation. Y= A+B
 
## Procedure
1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram.

6.Give the respective inputs for timing diagram and obtain the results

## Program:
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

Developed by: sivaram R
RegisterNumber:  212222100050
```
F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
module ex2(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1 = (~A)&(~B) & (~C) & (~D);
assign x2 = (A) & (~C) & (~D);
assign x3 = (~B) & (C) & (~D);
assign x4 = (~A) & (B) & (C) & (D);
assign x5 = (B) & (~C) & (D);
assign F1 = x1 | x2 | x3 | x4 | x5;
endmodule 

```
## TRUTH TABLE:
![ex2 tt](https://github.com/sivaram-R/Experiment--02-Implementation-of-combinational-logic-/assets/121165794/06051878-917d-4434-866a-a7109cc4d7c4)

## RTL DIAGRAM:
![RTL1](https://github.com/sivaram-R/Experiment--02-Implementation-of-combinational-logic-/assets/121165794/3109aeff-8262-4967-b27b-3c79b4b443d9)
## OUTPUT:
![2023-08-25 (2)](https://github.com/sivaram-R/Experiment--02-Implementation-of-combinational-logic-/assets/121165794/2b89a585-3d26-497c-9403-40796c8eba04)
## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
