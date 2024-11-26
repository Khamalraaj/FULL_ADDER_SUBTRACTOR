# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

**Procedure**

Write the detailed procedure here

**Program:**

Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.

FULL ADDER PROGRAM
```
module wel(A,B,Cin,S,C);
input A,B,Cin;
output S,C;
assign S=(A^B^Cin);
assign C=((A&B)|((A^B)&Cin));
endmodule
```
FULL SUBTRACTOR PROGRAM
```
module come(a,b,bin,diff,borr);
input a,b,bin;
output diff,borr;
assign diff=(a^b^bin);
assign borr=((~a&b)|((~a^b)&bin));
endmodule
```
Developed by:khamalraaj S

RegisterNumber: 24901015


**RTL Schematic**

LOGIC DIAGRAM FOR FULL ADDER
![Screenshot 2024-11-05 140859](https://github.com/user-attachments/assets/f1d2b2d0-6ee5-4f22-a9d0-486ae64757ac)
LOGIC DIAGRAM FOR FULL SUBTRACTOR
![Screenshot 2024-11-05 142651](https://github.com/user-attachments/assets/10c1fee4-db5b-431b-bf20-f92327a1509a)

**Output Timing Waveform**

FULL ADDER
![Screenshot 2024-11-05 141258](https://github.com/user-attachments/assets/22b1a107-0395-497f-83ab-adbce16005f7)
FULL SUBTRACTOR
![Screenshot 2024-11-05 142832](https://github.com/user-attachments/assets/c9b7bde2-e558-44cf-9792-05f2053945ee)

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



