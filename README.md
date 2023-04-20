# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 ## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.Combinational logic gates are digital circuits that produce outputs based solely on the current inputs. These gates are the building blocks for implementing digital systems and are used in a wide range of applications, including arithmetic and logic operations, memory devices, and control circuits.The two functions, F1 and F2, can be implemented using a combination of logic gates such as AND gates, OR gates, and NOT gates.


## Procedure:
1.Use module projname(input,output) to start the Verilog programmming.

2.Assign inputs and outputs using the word input and output respectively.

3.Use defined keywords like wire,assign and required logic gates to represent the boolean expression.

4.Use each output(RTL Viewer and Timing Diagram) to represent F1 and F2.

5.End the verilog program using keyword endmodule.
## Program:
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: Lavanya M
RegisterNumber:  212222110021


F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

module exp2f1(A,B,C,D,f1);
input A,B,C,D;
output f1;
assign f1=(~B&~D)|(A&B&~C)|(~A&B&D);
endmodule

F2=xy’z+x’y’z+w’xy+wx’y+wxy

module exp2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=(~y&z)|(x&y)|(w&y);
endmodule
/*

# Output:

## RTL DIAGRAM:

### F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

![rtl diagram exp(2)](https://user-images.githubusercontent.com/120103862/233444435-4818a840-64c2-483b-a579-1e721d4a128e.png)

### F2=xy’z+x’y’z+w’xy+wx’y+wxy

![rtl diagram exp 2(2)](https://user-images.githubusercontent.com/120103862/233444228-a12416d9-cc9c-4d53-8da7-1eb39e636955.png)


## Timing Diagram

### F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

![exp 2(1)](https://user-images.githubusercontent.com/120103862/233448490-bde5a4e7-3465-45cb-8e95-49a796d61035.png)

### F2=xy’z+x’y’z+w’xy+wx’y+wxy

![exp2(2)](https://user-images.githubusercontent.com/120103862/233446842-1ef9acbf-a8d4-459f-a747-f5e7aae8e322.png)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
