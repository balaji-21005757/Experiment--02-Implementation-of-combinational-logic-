# Experiment-02: Implementation of combinational logic

 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
```
F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
```
 
 
 
## Equipments Required:
1. Hardware – PCs, Cyclone II, USB flasher
2. Software – Quartus prime


## Theory:
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.
 

## Logic Diagram:
![image](https://github.com/SOMEASVAR/Experiment--02-Implementation-of-combinational-logic-/assets/93434149/a665c88c-10e7-4fca-b491-faf26b4f94b4)



## Procedure:
### Step 1:
Create a project with required entities.

### Step 2: 
Create a module along with respective file name.

### Step 3: 
Run the respective programs for the given boolean equations.

### Step 4:
Run the module and get the respective RTL outputs.

### Step 5: 
Create university program(VWF) for getting timing diagram.

### Step 6: 
Give the respective inputs for timing diagram and obtain the results.

## Program:
```
Program to implement the given logic function and to verify its operations in quartus using
Verilog programming.

Developed by: Balaji K
RegisterNumber:  212221230011
```
```
module Logic(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```
## RTL realization
![image](https://github.com/SOMEASVAR/Experiment--02-Implementation-of-combinational-logic-/assets/93434149/d395b283-1d45-4a3c-8a9a-cf8cbda4b891)
### Truth Table:
![image](https://github.com/SOMEASVAR/Experiment--02-Implementation-of-combinational-logic-/assets/93434149/4bd7dea9-6f7f-43c5-bab2-ee06b5bbd37e)


## Output:
## RTL
![image](https://github.com/SOMEASVAR/Experiment--02-Implementation-of-combinational-logic-/assets/93434149/1482e3d2-6216-4aff-aa23-34f87d9fb883)



## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
