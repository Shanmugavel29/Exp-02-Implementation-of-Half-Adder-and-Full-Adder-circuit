# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

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
### Program:
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: Shanmugavel.R.M
RegisterNumber:  
Half adder program:
module HalfAdder(A,B,sum,carry);
input A,B;
output sum,carry;
assign sum= A^B;
assign carry = A&B;
endmodule
Full adder program:
module FullAdder(A,B,Cin,sum,carry);
input A,B,Cin;
output sum,carry;
assign sum= A^B^Cin;
assign carry = (A&B)|((A^B)&Cin);
endmodule
```
### Output:
### RTL DIAGRAM:
## HALF ADDER:
![Screenshot 2023-09-14 183826](https://github.com/Shanmugavel29/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/114382660/1d37580c-8e7a-4f4f-b85f-1a81e87661c8)
## FULL ADDER:
![Screenshot 2023-09-14 183819](https://github.com/Shanmugavel29/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/114382660/06f7cfc3-d734-4f97-a622-c5bff20b3ece)
### TRUTH TABLE:
## HALF ADDER:
![Screenshot 2023-09-14 183751](https://github.com/Shanmugavel29/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/114382660/645ab5fd-b89c-4a61-befc-b58d4203a8f0)
## FULL ADDER:
![Screenshot 2023-09-14 183805](https://github.com/Shanmugavel29/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/114382660/eaaca43c-7e54-4e64-8e1f-d0149c1d0f96)
### WAVEFORM:
## HALF ADDER:
![Screenshot 2023-09-14 183738](https://github.com/Shanmugavel29/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/114382660/ca8fa401-ee94-4c27-b820-206085de45d6)
## FULL ADDER:
![Screenshot 2023-09-14 183706](https://github.com/Shanmugavel29/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/114382660/a4171e8c-5b77-4a3d-886e-efecfcb430fd)
### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
