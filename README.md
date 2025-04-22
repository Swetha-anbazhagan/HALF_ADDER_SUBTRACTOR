# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**

Half Adder:

![half_adder_tt1](https://github.com/user-attachments/assets/14f89243-97bf-476f-b44a-243640d34ffb)

Half  Subtracter:

![half_sub_tt1](https://github.com/user-attachments/assets/59dc7a5c-0d95-4840-a522-c1c0db62921c)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

```
Developed by:Swetha A
RegisterNumber:212224040343

HALF ADDER

module HA(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=(a^b);
assign carry=(a&b);
endmodule

HALF SUBTRACTER

module HS(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference=(a^b);
assign borrow=(~a&b);
endmodule

```
**RTL Schematic**

![WhatsApp Image 2025-04-22 at 23 25 43_02281874](https://github.com/user-attachments/assets/7490f9d9-0cc5-4a5a-81a7-94972b913aed)

![WhatsApp Image 2025-04-22 at 23 04 39_acdaae83](https://github.com/user-attachments/assets/8c43076d-0dd3-44ff-bb4f-24c8001139a3)

**Output/TIMING Waveform**

![WhatsApp Image 2025-04-22 at 23 23 53_d437af95](https://github.com/user-attachments/assets/106eb80a-2a2a-4bf4-a9fd-d939bd5b7815)

![WhatsApp Image 2025-04-22 at 23 04 39_f14799aa](https://github.com/user-attachments/assets/55d05165-8110-4a21-8bf3-f0fb3a0e5d6b)

**Result:**

  Thus,the Verilog program has been successfully executed.
