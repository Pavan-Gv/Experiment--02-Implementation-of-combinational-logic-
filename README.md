# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
```
F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
```
## Equipments Required:
```
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
```
## Theory
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

## Logic Diagram:

![image](https://github.com/Pavan-Gv/Experiment--02-Implementation-of-combinational-logic-/assets/94827772/83eabd61-5cac-463e-a9c1-48a57a217497)

## Procedure:
<b>Step 1</b>: Create a project with required entities.

<b>Step 2</b>: Create a module along with respective file name.

<b>Step 3</b>: Run the respective programs for the given boolean equations.

<b>Step 4</b>: Run the module and get the respective RTL outputs.

<b>Step 5</b>: Create university program(VWF) for getting timing diagram.

<b>Step 6</b>: Give the respective inputs for timing diagram and obtain the results.
## Program:
```
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: G Venkata Pavan Kumar
RegisterNumber: 212221240013
```
```
module Logic(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```
## RTL realization

![image](https://github.com/Pavan-Gv/Experiment--02-Implementation-of-combinational-logic-/assets/94827772/48c23c24-334f-4c49-8f5e-ab00d8f8623a)

## TruthTable:

![image](https://github.com/Pavan-Gv/Experiment--02-Implementation-of-combinational-logic-/assets/94827772/391d65f7-57f6-4d83-9210-85882fe3eef6)

## Output:
![image](https://github.com/Pavan-Gv/Experiment--02-Implementation-of-combinational-logic-/assets/94827772/b18445cf-e7d9-4c3d-bfde-af2bd100c5a7)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
