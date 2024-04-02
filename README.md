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


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Praveen K 

RegisterNumber:212223230153
```
module combinationalcircuit(A,B,C,D,F1);
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
![image](https://github.com/K-PRAVEEN-2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742724/024b8563-a6bc-4f56-9d86-449e7dde668d)



**RTL realization**

**Output:**

**RTL**
![image](https://github.com/K-PRAVEEN-2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742724/90e006a0-db30-4cb2-8b89-718b6ca63a39)

**Timing Diagram**
![image](https://github.com/K-PRAVEEN-2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742724/59a8a7d3-a1c4-4d77-8655-9d9e5d7521ed)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

