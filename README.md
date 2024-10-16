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
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Sana Fathima H
RegisterNumber:212223240145
*/
```
module ex02 (E,F,A,B,C,D);
input A, B, C, D; output E,F;
assign E = A || (B && C) || ((!B) && D);
assign F=((!B) && C) || ( B && (!C) && (!D));
endmodule

```
**Truth Table**
![image](https://github.com/user-attachments/assets/87a11a12-2d6e-43c7-9974-6b2668238b9e)


**RTL realization**
![image](https://github.com/user-attachments/assets/1b078ed5-9806-4b43-9ff4-e8412ad2150a)



**Output:**
RTL
Timing Diagram
![image](https://github.com/user-attachments/assets/26cc61a4-0859-4b1f-a3d6-d5fa0d404a69)




**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

