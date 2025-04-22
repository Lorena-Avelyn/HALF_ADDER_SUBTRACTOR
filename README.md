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
![WhatsApp Image 2025-04-22 at 23 04 11_1c1d7bab](https://github.com/user-attachments/assets/1fa8aacf-4f27-4232-9528-b5c1d1a91a98)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
```
Developed by:Lorena-Avelyn
RegisterNumber:212224040174

HALF ADDER

module HA(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=(a^b);
assign carry=(a&b);
endmodule

HALF SUBTRACTOR

module HS(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference=(a^b);
assign borrow=(~a&b);
endmodule

```

**RTL Schematic**

![Screenshot 2025-04-22 232529](https://github.com/user-attachments/assets/e0f2d62f-b5a7-4e9d-9e4a-ee9b81c8c5b2)
![Screenshot 2025-04-22 230501](https://github.com/user-attachments/assets/9831780d-a9bd-4819-a0e0-8e1c0ca79f77)


**Output/TIMING Waveform**

![Screenshot 2025-04-22 232404](https://github.com/user-attachments/assets/15912f31-e76c-4e29-8dbd-0fac52ee6ba2)
![Screenshot 2025-04-22 230440](https://github.com/user-attachments/assets/1ef128a8-8b52-4e5a-9286-18452e7aa333)

**Result:**

Thus the half adder and half subtractor are studied and the truth table table,logic gates are verified in Quartus II using Verilog programming.
