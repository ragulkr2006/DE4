## NAME: RAGUL K R
## REG.NO:24900660
## EXP.NO:4-FULL_ADDER_SUBTRACTOR

# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

*AIM:*

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

*Equipments Required:*

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

*Full Adder and Full Subtractor*

*Full Adder*

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

*Figure -1 FULL ADDER*

*Full Subtractor*

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

*Truthtable*

FULL ADDER

![WhatsApp Image 2024-11-28 at 10 56 35_0ebe3f68](https://github.com/user-attachments/assets/fe460178-70b1-445e-bfb2-2e7fdfb020f0)


FULL SUBTRACTOR

![WhatsApp Image 2024-11-28 at 10 56 47_43251b5a](https://github.com/user-attachments/assets/20bab93e-9726-427d-a788-7c7622f515a9)




*Program:*
*DEVELOPED BY: RAGUL K R*
*REG NO : 24900660*


i)FULL ADDER

module fa(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=( (a ^ b)^cin);
assign carry= ( (a & b)| ( cin &(a ^ b )));
endmodule


ii)FULL SUBTRACTOR

module fs(a,b,bin,difference,borrow);
input a,b,bin;
output difference,borrow;
assign difference= ( (a ^ b)^bin);
assign borrow= ( ( a & b)| ( bin & (a ^ b )));
endmodule

*RTL Schematic*

FULL ADDER

![WhatsApp Image 2024-11-28 at 10 29 44_895b90c7](https://github.com/user-attachments/assets/e2a4fa9b-f464-4fe2-8480-a17ea3ffba71)



FUL SUBTRACTER

![WhatsApp Image 2024-11-28 at 10 46 53_6713f588](https://github.com/user-attachments/assets/1173558c-d8f8-4990-8248-999663fdce5b)



*Output Timing Waveform*

FULL ADDER

![WhatsApp Image 2024-11-28 at 10 28 57_0b341032](https://github.com/user-attachments/assets/8780ea0e-dd52-4e1a-8fec-d4906aece85a)



FULL SUBTRACTER

![WhatsApp Image 2024-11-28 at 10 45 39_0d54dd53](https://github.com/user-attachments/assets/25d9a9a4-9b5e-456a-8acb-20ed4407053b)



*Result:*

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.
