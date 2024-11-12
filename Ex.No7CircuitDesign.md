# Ex.No: 7  Logic Programming –  Logic Circuit Design
### DATE:                                                                            
### REGISTER NUMBER : 
### AIM: 
To write a logic program to design a circuit like half adder and half subtractor.
###  Algorithm:
1. Start the Program
2. Design a AND gate logic if both inputs are 1 then output is 1.
3. Design a OR gate logic if any one of input is 1 then output is 1.
4. Design a XOR gate logic if both inputs are different then output is 1.
5. Design a NOT gate logic if input is 0 then output is 1.
6. Design a half adder and half subtractor using the rules.
7. Test the logic.
8. Stop the program.

### Program:
half_adder(A, B, Sum, Carry) :-

Sum is (A + B) mod 2,

Carry is (A + B) // 2.
half_subtractor(A, B, Difference, Borrow) :-

Difference is (A - B) mod 2,

Borrow is (A - B) // 2.
full_adder(A, B, CarryIn, Sum, CarryOut) :-

TempSum is (A + B + CarryIn) mod 2,

CarryOut is (A + B + CarryIn) // 2,

Sum is TempSum.
full_subtractor(A, B, BorrowIn, Difference, BorrowOut) :-

TempDiff is (A - B - BorrowIn) mod 2,

BorrowOut is (A - B - BorrowIn) // 2,

Difference is TempDiff.










### Output:
![image](https://github.com/user-attachments/assets/afbce05f-c428-4be7-95c2-b2c85660cb54)
![image](https://github.com/user-attachments/assets/df9a95e5-7fe8-4e6a-bb1c-3e76acd82c2e)
![image](https://github.com/user-attachments/assets/ddff12bc-8fca-4a6b-b328-f8e0ceaefd9c)
![image](https://github.com/user-attachments/assets/f728dcde-76ff-437f-91fe-1224173d12bd)



### Result:
Thus the truth table of circuit verified sucessfully.
