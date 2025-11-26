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

Half Adder 

![Half adder truthtable](https://github.com/user-attachments/assets/c4bd337c-127f-45ed-8302-aedb93eb7473)

Half Subtractor

![WhatsApp Image 2025-11-26 at 22 24 22_7d4325ba](https://github.com/user-attachments/assets/a4487d47-40d1-4476-91e8-42dc9e1d5c6c)




**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Half Adder

    module half_adder (

    input wire a,b,    //Inputs
    
    output wire sum,    //Sum output
   
    output wire carry    //Carry output
   
    );

    // Logic equations
   
    assign sum   = a ^ b;    // XOR for Sum
   
    assign Carry = a & b;    //AND for Carry
   
    endmodule


Half Subtractor


    module half_subtractor (

    input wire a, b,          //Inputs
   
    output wire diff, borrow  //Outputs
   
    );

    // Logic equations 
   
    assign diff   = a ^ b;        //  XOR for difference
    
    assign borrow = ~a & b;       // Borrow when a < b
      
    endmodule

Developed by:PRASANNA V RegisterNumber:25008398

**RTL Schematic**

Half Adder

![Half adder](https://github.com/user-attachments/assets/288db878-9454-465c-ab89-6ba8eb431676)

Half Subtractor

![Half Subtractor](https://github.com/user-attachments/assets/ef3fda57-d69c-47f1-acfb-2596c55d6474)


**Output/TIMING Waveform**

Half Adder

![Adder Timing](https://github.com/user-attachments/assets/f86e2198-2031-4653-9606-345547b95b03)

Half Subtractor

![Adder Timing](https://github.com/user-attachments/assets/67083055-2d25-494e-8aa5-6decd3fd1da8)



**Result:**

Designing a half adder and half subtractor circuit and verifying its truth table in Quartus using Verilog programming is created successfully.

