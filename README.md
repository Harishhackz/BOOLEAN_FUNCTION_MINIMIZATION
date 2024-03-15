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

Developed by:HARISH B RegisterNumber:212223040061
```
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

```


**RTL realization**
![312535957-dbd64921-6857-40ee-a21b-55fa17e9f89b](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/147088495/597baa03-d4a4-4232-a56e-66410d9a06d7)

**Output:**
![DE](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/147088495/8eb70650-c195-43ab-8323-4cbb52eeb9e7)

**Timing Diagram**
![DE12](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/147088495/52d7922c-2ba0-465d-a1bb-36e0b529f10d)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

