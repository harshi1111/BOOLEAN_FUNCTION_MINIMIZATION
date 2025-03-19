### NAME : HARSHITHA V
### REGISTER NO : 212223230074
### EXP 2: BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**


**Procedure:**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
module experiment2(a,b,c,d,w,x,y,z,f2,f1);
input a,b,c,d;
output f1;
assign f1 = ((~a & ~b & ~c & ~d) | (a&(~c)&(~d))| ((~b)&c&(~d)) | ((~a)&b&c&d) | (b&(~c)&d));
input w,x,y,z;
output f2;
assign f2=((x&(~y)&z) | ((~x)&(~y)&z) | ((~w)&x&y) | (w&(~x)&y) | (w&x&y));
endmodule
```


**RTL realization:**



![image](https://github.com/user-attachments/assets/5e5d82c0-7a97-4e2e-99c6-301f21f20b71)



**RTL:**

![image](https://github.com/user-attachments/assets/51e4124c-7ab3-40d7-be9e-d2155975c8ff)




**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

