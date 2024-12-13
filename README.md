# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions

**Logic Diagram**

i)F1 TRUTHTABLE:


![Screenshot 2024-12-13 123617](https://github.com/user-attachments/assets/f549e226-4360-455a-8645-47d063df70db)

ii)F2 TRUTHTABLE


![Screenshot 2024-12-13 123722](https://github.com/user-attachments/assets/59a24a61-39f8-4a5c-99ec-4636dfabf887)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:MOHAMED ARSHADULLAH

RegisterNumber:24005938
*/
```
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
assign f2=((~y & z)|( w & y )|(x & y));0
endmodule

```


**RTL**


![exp02f1 (2)](https://github.com/user-attachments/assets/06031ed1-5dfd-4370-b3a5-e15d132dc315)


![exp02f2](https://github.com/user-attachments/assets/930500ea-1d3e-48f3-8230-a4cb5d3a00a0)

**Output:**


![output 02](https://github.com/user-attachments/assets/658a8608-c601-45f3-895a-fe825fae663f)



![output 2-2](https://github.com/user-attachments/assets/b4e73158-5e42-4200-b712-54ac959a6218)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

