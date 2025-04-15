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
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```


**RTL realization**

**Output:**

**RTL**

Boolean function minimization f1


![image](https://github.com/user-attachments/assets/eb9ca480-0419-4bfa-b842-8d36e59dced1)

Boolean function minimization f2

![image](https://github.com/user-attachments/assets/33f3b362-ead3-447e-b7ad-fd64e133007c)





**Timing Diagram**
Boolean function minimization f1


![image](https://github.com/user-attachments/assets/d4423c3c-a204-4ca1-b220-e186c66cdedf)

Boolean function minimization f2

![image](https://github.com/user-attachments/assets/b0a27df8-462e-425d-9df6-1267e4810ca8)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

