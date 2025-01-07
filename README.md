## NAME: RAGUL K R
## REG.NO:24900660
## EXP.NO:4-IMPLEMENTATION OF FULL ADDER AND FULL SUBRACTOR CIRCUIT


## AIM:

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming..

## Equipments Required:

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime  

## Full Adder and Full Subtractor

## Full Adder:

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

*Figure -1 FULL ADDER*

## Full Subtractor:

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

## Truthtable

FULL ADDER

![WhatsApp Image 2024-11-28 at 10 56 35_0ebe3f68](https://github.com/user-attachments/assets/fe460178-70b1-445e-bfb2-2e7fdfb020f0)


FULL SUBTRACTOR

![WhatsApp Image 2024-11-28 at 10 56 47_43251b5a](https://github.com/user-attachments/assets/20bab93e-9726-427d-a788-7c7622f515a9)

## procedure :

## full Adder 
1.open quartus II and create A new project.
2.use schematic design entry to draw the full adder circuit .
3.The circuit consist of XOR,AND and OR gates.
4.compile the design,verify its functionality through simulation.
5.implement the design on the target device and program it .


## Full Subractor :
1.follow the same steps as for the full adder .
2.draw the full subractor circuit  using schematic design .
3.the circuit includes XOR,AND,OR gates to perform subraction.
4.compile ,simulate,implement,and program the design similarly to the full adder .

## program :
![WhatsApp Image 2025-01-07 at 08 28 28_194bd2ac](https://github.com/user-attachments/assets/e07dcb6e-0c9b-445b-b382-b0ceb5be23b0)



## RTL viewer:
![WhatsApp Image 2025-01-06 at 05 19 13_aea971c0](https://github.com/user-attachments/assets/dcefe4c7-53cd-40d0-8b80-52f4cd254839)



## Output Timing Waveform:
![WhatsApp Image 2025-01-06 at 05 17 54_f9a5e269](https://github.com/user-attachments/assets/d2421881-f0ad-48af-9516-c2e47589cddf)


## Result:

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.
