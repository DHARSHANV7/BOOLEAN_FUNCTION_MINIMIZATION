# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**


![Screenshot 2025-03-21 075546](https://github.com/user-attachments/assets/2b7a3a39-2d6f-45dc-a7c9-7e25099fe67a)
![Screenshot 2025-03-21 075555](https://github.com/user-attachments/assets/1e61f8c1-6315-4435-884a-adb6bf2e6c75)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
module EXP_3_1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b&~d)|(~a&b&d)|(a&b&~c));
endmodule
```

```
module EXP_3_2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y&z)|(x&y)|(w&y));
endmodule
```

Developed by: Dharshan V

RegisterNumber: 212224240035


**RTL realization**
![Screenshot 2025-03-21 075018](https://github.com/user-attachments/assets/b02660a4-f222-4ecb-bd9b-42f85489bb4d)
![Screenshot 2025-03-21 075033](https://github.com/user-attachments/assets/7484b248-4ff8-4f86-8282-6ebed8e245b6)


**Timing Diagram**
![Screenshot 2025-03-21 075118](https://github.com/user-attachments/assets/db4fba33-9a8c-4307-bbcd-6c20066170c0)
![Screenshot (174)](https://github.com/user-attachments/assets/03c53752-5cca-4cad-a445-fda13706ff14)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

