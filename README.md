# EXP-04-IMPLEMENTATION OF HALF ADDER AND FULL ADDER CIRCUIT
# AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

# Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
# Theory:
Adders are digital circuits that carry out addition of numbers.

## Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

## Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

# Procedure

1.Connect the supply (+5V) to the circuit     

2.Switch ON the main switch

3.If the output is 1, then the led glows.
# Program:
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: SIVAMOHANASUNDARAM.V
RegisterNumber: 212222230145

1. Program to design a half adder:

module ex3(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=a^b;
assign carry=a&b;
endmodule 

2. Program to design a full adder:

module ex31(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=a^b^cin;
assign carry=(a&b)|((a^b)&cin);
endmodule

```
# TRUTH TABLE:
## HALF ADDER:
![de1](https://github.com/SivaMohan-cloud/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/121418870/d8636349-18f2-4083-b9aa-79ccc80d0c93)

## FULL ADDER:
![de2](https://github.com/SivaMohan-cloud/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/121418870/e76b6675-46eb-488f-af67-66ae1041800a)

# RTL REALIZATION :
## HALF ADDER:
![de3](https://github.com/SivaMohan-cloud/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/121418870/f3f7262c-b5ec-4513-b3c7-4787e44fd390)

## FULL ADDER:
![de4](https://github.com/SivaMohan-cloud/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/121418870/459b13ef-139d-4072-8010-a37d61edc26f)

# OUTPUT WAVEFORM:
## HALF ADDER:
![de5](https://github.com/SivaMohan-cloud/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/121418870/b1200049-82ad-4441-8e5f-be9cfaa716b7)

## FULL ADDER:
![de6](https://github.com/SivaMohan-cloud/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/121418870/14e20d59-71e8-4044-a8cb-df4966a6286d)

# Result:
Thus the half adder and full adder circuit are designed and the truth table for half adder and full adder are verified.
