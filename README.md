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
module experiment2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&`d|(~a&b&d)|(a&b&~c)));
assign f2=((~y&z)|(x&y)|(w&y));
endmodule
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:*/


**RTL realization**


![Screenshot 2024-11-05 105136](https://github.com/user-attachments/assets/aab23f23-e995-4f52-a04a-48112cd38e1d)

**Output:**

**RTL**

**Timing Diagram**

![Screenshot 2024-11-05 105036](https://github.com/user-attachments/assets/5ff9d398-4b6d-4398-a833-b26d567ccca1)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

