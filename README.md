# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

F2=xy’z+x’y’z+w’xy+wx’y+wxy

Equipment Required:

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime Procedure

Type the program in Quartus software.

Compile and run the program.

Generate the RTL schematic and save the logic diagram.

Create nodes for inputs and outputs to generate the timing diagram.

For different input combinations generate the timing diagram.

Program:

module exp22(A,B,C,D,F1);
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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

Developed by:L.yagnesh kumar reddy
regi:212223100024

Logic Diagram 
![Screenshot 2024-03-24 131640](https://github.com/23004742/BOOLEAN_FUNCTION_MINIMIZATION/assets/150319318/3e9a8700-b6a3-4a80-87d6-4a2d7796c875)

RTL realization 
![Screenshot 2024-03-24 131647](https://github.com/23004742/BOOLEAN_FUNCTION_MINIMIZATION/assets/150319318/47e6f2a7-8fb1-4968-85c8-a469fc3b1592)

Output: truthtable 
![Screenshot 2024-03-24 131702](https://github.com/23004742/BOOLEAN_FUNCTION_MINIMIZATION/assets/150319318/4428dc81-56c0-4b69-a720-f80534c18f54)

Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


