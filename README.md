# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
#Program:
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: YUVARAJ B 
RegisterNumber: 212222230182 

Half Adder:
module halfadder(A,B,sum,carry);
input A,B;
output sum,carry;
assign sum=A^B;
assign carry=A&B;
endmodule

Full Adder:
module Fulladder(A,B,Cin,sum,carry);
input A,B,Cin;
output sum,carry;
assign sum= A^B^Cin;
assign carry = (A&B)|((A^B)&Cin);
endmodule
```


### Output Waveform:
HALF ADDER:

![264914112-df8c47c7-743e-43ce-b9bf-b65de203e935](https://github.com/Yuva2005raj/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118343998/3710d0af-23fb-497e-8e6a-c8782d691f7b)

FULL ADDER:

![264914178-b6bfaa14-2e76-47dd-b18f-ee3490fa2703](https://github.com/Yuva2005raj/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118343998/77012921-af23-4a8d-9bf8-9f85219cb9fb)

### RTL DIAGRAM:
HALF ADDER:

![264914237-b140583c-4278-41d9-aeca-3c8c12143eed](https://github.com/Yuva2005raj/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118343998/7b45563c-7d0c-47fe-b223-1e32c558d783)

FULL ADDER:

![264914259-f1ee68dc-3f13-4034-9891-d475e263f70e](https://github.com/Yuva2005raj/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118343998/e12d1eea-5a66-41eb-a90f-c82d1fbd5269)


### TRUTH TABLE
HALF ADDER:

![264914855-a20b8f13-a65c-41ce-816e-960026574f46](https://github.com/Yuva2005raj/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118343998/476346a3-e023-46f9-99a2-ca5771b286b8)

FULL ADDER:

![264916574-60ea1f9b-1a0d-4cac-8df5-634db3638782](https://github.com/Yuva2005raj/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118343998/e8258a92-32d6-4fab-8718-033d1e33b63d)


### Result:
Thus the half adder and full adder circuits are designed and the truth tables is verified using quartus software.
