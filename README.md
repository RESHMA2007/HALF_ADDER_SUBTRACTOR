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

![Screenshot 2024-12-07 152507](https://github.com/user-attachments/assets/fbcc70ef-9971-4ea2-a2af-e9c9cac49536)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

![Screenshot 2024-12-07 154204](https://github.com/user-attachments/assets/71328c85-6bf0-447b-978f-c2006da03315)

**Truthtable**
(i)HALF ADDER
![Screenshot 2024-12-07 154804](https://github.com/user-attachments/assets/5a26002a-5001-4c25-ab09-af0de6a0d114)
(ii)HALF SUBTRACTOR
![Screenshot 2024-12-07 154843](https://github.com/user-attachments/assets/1516d080-9180-455d-b947-edb98410fb85)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:Reshma R RegisterNumber:24900406
```
(i)HALF ADDER
module halfadd(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=(a^b);
assign carry= (a&b);
endmodule

(ii)HALF SUBTRACTOR
module hs(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference=(a^b);
assign borrow= (~a&b);
endmodule
```

**RTL Schematic**

**Output/TIMING Waveform**
(i)HALF ADDER
![Screenshot 2024-12-07 152834](https://github.com/user-attachments/assets/c2a930c7-2560-4d2e-935e-702b2cd08995)
(ii)HALF SUBTRACTOR
![Screenshot 2024-12-07 154403](https://github.com/user-attachments/assets/3f1600cf-4c48-45b3-94d7-36faf7d31ca7)


**Result:**
Thus the given logic functions are implemented using and their operations are verified using.
