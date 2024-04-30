# EXPERIMENT : HALF_ADDER_SUBTRACTOR
# DATE :

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
![DE E-3 truthtable](https://github.com/04Varsha/HALF_ADDER_SUBTRACTOR/assets/149035374/c06bba9c-9c1e-4e92-a1e3-869583ce44c7)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
~~~
module EX03(a,b,sum,carry,D,Bo); 
input a,b; 
output sum,carry,D,Bo;
xor g1(sum,a,b);
and g2(carry,a,b); 
wire abar; 
not g3(abar,a); 
xor g4(D,a,b); 
and g5(Bo,abar,b); 
endmodule

Developed by: S.HARISH
RegisterNumber: 212223040062
~~~

*/


**RTL Schematic**

![318335096-90716de4-b5ed-4674-98d5-51daa65ac1f7](https://github.com/04Varsha/HALF_ADDER_SUBTRACTOR/assets/149035374/217ae264-d9ba-4625-bd4f-555dd8bdaf61)

**Output/TIMING Waveform**

![318335195-5ac0a2d5-9c87-4c85-9109-76a689d6d841](https://github.com/04Varsha/HALF_ADDER_SUBTRACTOR/assets/149035374/0c936ddf-4579-4971-805e-0393520e814a)

**Result:**
Implementation-of-Half-Adder-and-Half Subtractor-circuit is excuted sucessfully.
