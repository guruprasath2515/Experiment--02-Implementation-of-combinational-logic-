# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:
````
module kmap(a,b,c,d,w,x,y,z,F1,F2);
input a,b,c,d,w,x,y,z;
output F1,F2;
wire A1,A2,A3,B1,B2,B3;
assign A1=(~a&(~b)&(~c)&(~d));
assign A2=(a&c&(~d));
assign A3=((~b)&c&(~d));
assign F1=A1|A2|A3;
assign B1=(x&(~y)&z);
assign B2=(~x&(~y)&z);
assign B3=(~w&x&y);
assign F2=B1|B2|B3;
endmodule
````
## RTL realization
![image](https://github.com/guruprasath2515/Experiment--02-Implementation-of-combinational-logic-/assets/155418874/47941bb8-39dd-4e2d-b758-8ebd75be3e21)
## Truth table
![WhatsApp Image 2024-01-02 at 14 07 04_47687bea](https://github.com/guruprasath2515/Experiment--02-Implementation-of-combinational-logic-/assets/155418874/97b973e9-bdb1-4c77-b52e-b4665f3c74f9)

## WAVE FORM
![WhatsApp Image 2024-01-02 at 14 09 04_2e01285b](https://github.com/guruprasath2515/Experiment--02-Implementation-of-combinational-logic-/assets/155418874/a2d4e3b9-4270-4c50-8029-2345bb058f38)



## Output:
## RTL
## Timing Diagram
## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
