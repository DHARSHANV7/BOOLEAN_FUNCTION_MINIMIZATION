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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming./


Developed by: Dharshan V

RegisterNumber: 212224240035
```
module exp2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

module exp22(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```
**Output:**

**RTL**
![Screenshot 2025-03-18 205833](https://github.com/user-attachments/assets/9a351987-210d-483a-89a6-22d283e8eb68)
![Screenshot 2025-03-18 211245](https://github.com/user-attachments/assets/51e89129-d92e-4037-a80e-57af3d512a09)


**Timing Diagram**
![Screenshot 2025-03-18 210040](https://github.com/user-attachments/assets/80c85123-284c-44ee-8561-a50df9cbf2a8)
![Screenshot 2025-03-18 211613](https://github.com/user-attachments/assets/1ef0b161-5b87-48b7-b2cb-b8101a26209e)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

