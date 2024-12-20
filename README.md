**Developed by: Naveen R** 

**RegisterNumber: 24900811**

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
```
module Expt2(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule
```
**LOGIC SYMBOL & TRUTH TABLE:**

![Screenshot 2024-11-29 112847](https://github.com/user-attachments/assets/1806ab50-639e-438c-8448-8d8dd7d8865f)

   ![Screenshot 2024-11-29 112931](https://github.com/user-attachments/assets/0d813979-7ee9-4b3e-b54a-d105e9546f19)




**RTL realization**:
![Screenshot (17)](https://github.com/user-attachments/assets/72b088aa-fd23-4266-af2a-52356b100e88)


**Output:**
![Screenshot (16)](https://github.com/user-attachments/assets/96151f38-373e-42d0-9198-fd3565afa923)




**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

