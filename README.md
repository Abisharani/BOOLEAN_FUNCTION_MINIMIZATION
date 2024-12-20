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
![minimizaton-boolean-gate](https://github.com/user-attachments/assets/81e1e61a-dd6c-4ec8-82d5-1e1066f0fa13)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
Developed by:ABISHA RANI S
RegisterNumber:24900748
```
*/
```
*/
i)
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

ii)
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```
*/
**RTL realization**


![Screenshot (3)](https://github.com/user-attachments/assets/25bb0d31-2e08-4a12-bd41-b0ee645a6c87)
![Screenshot (10)](https://github.com/user-attachments/assets/7b9c2567-0392-493d-b184-726c2237fee2)



**Timing Diagram**

![Screenshot (20)](https://github.com/user-attachments/assets/64435942-8438-4f16-9421-dd50eadab7e9)
![Screenshot (21)](https://github.com/user-attachments/assets/a0475c1c-4035-45d1-9980-f632438e92a8)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

