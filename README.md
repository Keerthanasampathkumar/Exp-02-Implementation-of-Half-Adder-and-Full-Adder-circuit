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
#### Figure -01 HALF ADDER 

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -02 FULL ADDER 

![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

### Procedure

Connect the supply (+5V) to the circuit

Switch ON the main switch

If the output is 1, then the led glows.
### Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: KEERTHANA S

RegisterNumber:  212222230066

### PROGRAM 1

module Halfadder(a,b,sum,carry);

input a,b;

output sum,carry;

xor(sum,a,b);

and(carry,a,b);

endmodule
### PROGRAM 2
module fulladd(a,b,c,sum,carry);

input a,b,c;

output sum,carry;

assign sum=((a^b)^c);

assign carry=((a&b)|(b&c)|(c&a));

endmodule 
*/

### OUTPUT:
### RTL
![1](https://user-images.githubusercontent.com/119477890/231788895-29f3b77b-ac05-4716-9982-e17736643077.png)
![2](https://user-images.githubusercontent.com/119477890/231788928-b9e0b66d-bc72-4371-b0cb-9c2fb66597ec.png)
### TIMING DIAGRAM
![3](https://user-images.githubusercontent.com/119477890/231788999-7bbf4707-b470-45f4-90c8-3035732c9854.png)
![4](https://user-images.githubusercontent.com/119477890/231789156-fd11b2ff-6947-4e74-98a3-df6bbca2f6ab.png)
### TRUTHTABLE
![Truthtable 0](https://user-images.githubusercontent.com/119477890/231785577-8fa1c9bd-34f8-49f2-9eef-7d6c188731ee.png)
![tt](https://user-images.githubusercontent.com/119477890/231782570-d4fef1b3-7cd1-45ed-8683-a575e4b73560.png)

### Result:
Thus,the output for the half adder and full adder are successfully done
