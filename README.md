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

**1) .**

![F1](https://github.com/user-attachments/assets/ae5dff15-a63c-4ad6-a510-18205278f2df)

**2) .**

![F2](https://github.com/user-attachments/assets/c53fcedf-1baf-4803-912a-a3a02332bc38)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:** 

Developed by: Dharshan V

RegisterNumber: 212224240035

**1) .**
```
module ex2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1 = ((~b&~d)|(~a&b&d)|(a&b&~c));
endmodule 
```
**2) .**
```
module ex2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2 = ((~y&z)|(w&z)|(x&y)|(w&y&~z));
endmodule 
```
**Output:**

**1) .**

![image](https://github.com/user-attachments/assets/75e17e45-82d4-487f-a16f-fa604407d299)

**2) .**

![image](https://github.com/user-attachments/assets/a054cb4f-1e95-4c55-9e76-012e1302d576)


**RTL**

**Timing Diagram**

**1) .**

![image](https://github.com/user-attachments/assets/3f806e78-e83e-440a-94fb-0fcc3682df37)

**2) .**

![image](https://github.com/user-attachments/assets/47cc7085-016f-4dee-8bd5-04f9a0d16197)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

