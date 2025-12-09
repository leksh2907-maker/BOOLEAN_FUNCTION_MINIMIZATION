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

**RTL realization**
<img width="1389" height="667" alt="Screenshot 2025-12-09 234253" src="https://github.com/user-attachments/assets/3db530fe-0dfd-4e9d-afe0-864394358906" />


**Output:**
<img width="1386" height="707" alt="Screenshot 2025-12-09 234344" src="https://github.com/user-attachments/assets/35adce7c-13a4-47e2-9034-58652e502f9b" />
<img width="1386" height="713" alt="Screenshot 2025-12-09 234418" src="https://github.com/user-attachments/assets/dcf2ec4d-d16d-4268-a920-aec2d11957d2" />

**RTL**
<img width="1474" height="785" alt="image" src="https://github.com/user-attachments/assets/6c198a0f-38d3-414c-a329-db166cda312b" />
<img width="1369" height="732" alt="image" src="https://github.com/user-attachments/assets/525cfe35-d48d-4694-b74e-a203f34fe9fa" />

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

