# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**




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
```
module ex2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d) | (a & b & ~c) | (~a & b & d));
endmodule

```
```
module ex2m2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2= ((~y&z)|(w&y)|(x&y));
endmodule
```



**RTL realization**
F1
![image](https://github.com/user-attachments/assets/f031e34e-340b-46b6-b7bd-835956e6cb71)

F2
![image](https://github.com/user-attachments/assets/2b6ece49-d879-47e9-884c-3f7daf819025)



**Output:**
F1
![image](https://github.com/user-attachments/assets/6ecfa4a0-21eb-4de0-a2f7-9faf0cef6a6c)
F2
![image](https://github.com/user-attachments/assets/d100cb75-9733-40d1-8866-99ab1b092249)






**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

