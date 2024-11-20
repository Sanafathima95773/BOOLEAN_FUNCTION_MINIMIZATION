# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

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
module de_exp_2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d) | (a & b & ~c) | (~a & b & d));
endmodule

```
```
module proj23(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2= ((~y&z)|(w&y)|(x&y));
endmodule
```
**TRUTH TABLE**

F1
![image](https://github.com/user-attachments/assets/1557f0c2-fbb6-42e1-b1f1-dd1cc245dbde)


F2

![Screenshot 2024-11-20 160948](https://github.com/user-attachments/assets/d6788986-8f5e-4ffb-85de-18ee9df1fb0b)







**RTL realization**

F1

![image](https://github.com/user-attachments/assets/390dee0a-6285-4af9-94f3-aa0d18d09bd1)


F2

![image](https://github.com/user-attachments/assets/2b6ece49-d879-47e9-884c-3f7daf819025)



**Output:**

F1

![image](https://github.com/user-attachments/assets/08ba5e9e-087e-48dc-acbd-6861f4582a0c)


F2

![image](https://github.com/user-attachments/assets/ddfce599-fb32-4695-bd54-e4296250389f)








**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

