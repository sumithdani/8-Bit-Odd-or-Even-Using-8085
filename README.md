# 8-Bit-Odd-or-Even-Using-8085

## Aim:
To write an 8085 microprocessor program to check whether a given 8-bit number is odd or even.

## Apparatus Required:
•	Laptop with an internet connection

## Algorithm:
1.	Load the number from a specified memory location into register A.
2.	Perform an AND operation with 01H to check the least significant bit (LSB).
3.	If the result is 0, the number is even; otherwise, it is odd.
4.	Store the result in a specific memory location (odd or even flag).


## Program:
~~~
LDA 4200H
ANI 01H
JZ L1
MVI A, 01H
JMP L2
L1: MVI A,02H
L2: STA 4201H
HLT
~~~

## Output:
<img width="307" height="528" alt="Screenshot 2026-02-06 091049" src="https://github.com/user-attachments/assets/0d443065-e56d-4de4-a20d-09c36604694b" />
<img width="651" height="610" alt="Screenshot 2026-02-06 092125" src="https://github.com/user-attachments/assets/7835ea4b-44cf-4e82-b825-3a47fbf43775" />


<img width="303" height="549" alt="Screenshot 2026-02-06 091109" src="https://github.com/user-attachments/assets/934c39f3-6841-44ca-90c0-c8dfc0729b1e" />


## Result:
The 8085 microprocessor successfully checks whether a given number is odd or even and stores the result in memory.

