# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

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

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### Program:
~~~
Half Adder:
module halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b)
endmodule

Full Adder:
module halfadder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c
endmodule
Developed by: Monika D
RegisterNumber: 23013746  
~~~
### Truth table:
Half Adder Circuit:

![Screenshot 2023-12-13 023944](https://github.com/dhanamoni/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151629757/e5b46df2-82da-4f5c-8101-b7aa08b8680e)

Full Adder Ciruit:

![Screenshot 2023-12-13 024106](https://github.com/dhanamoni/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151629757/56f7f85f-c4f5-4b94-a479-b33177f63870)

### RTL realization:
Half Adder Circuit:

![Screenshot 2023-12-13 024233](https://github.com/dhanamoni/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151629757/e9ad806a-69c3-4578-b4d9-05b055e2a14c)

Full Adder Circuit:

![Screenshot 2023-12-13 024357](https://github.com/dhanamoni/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151629757/2f4173a1-eacf-487b-9bad-50e456606ed6)

### Output waveform:
Half Adder Circuit:

![Screenshot 2023-12-13 024535](https://github.com/dhanamoni/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151629757/bec02bff-dc12-497f-8b99-5a11c847753d)

Full Adder Circuit:

![Screenshot 2023-12-13 024550](https://github.com/dhanamoni/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151629757/5e96961b-ce7f-4246-b321-e6b6215e942a)

### Result:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming
