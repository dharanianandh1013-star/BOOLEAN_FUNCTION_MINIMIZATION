# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
Boolean function minimization is the process of simplifying complex Boolean expressions to their most efficient form while preserving their logical function. The goal is to reduce the number of logic gates, literals, and wiring needed for implementation in digital circuits, leading to lower costs, improved speed, and reduced power consumption.

**Logic Diagram**
![WhatsApp Image 2025-11-19 at 20 32 04_7936f598](https://github.com/user-attachments/assets/2bfdbfaf-09c9-4dbf-a0f9-efa99fd99388)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
module DAY27(a,b,c,d,f1,w,x,y,z,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
assign f2=((~y & z)|( w & y )|(x & y));
endmodule

**RTL realization**

**Output:**

**RTL**
<img width="1920" height="1080" alt="Screenshot (32)" src="https://github.com/user-attachments/assets/d8115538-fb7f-4fe4-921a-e7f0e98673fa" />

**Timing Diagram**
![WhatsApp Image 2025-11-19 at 20 29 11_2698767e](https://github.com/user-attachments/assets/67248776-eca3-4e6c-8432-91447ff308af)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

