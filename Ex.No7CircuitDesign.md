## Ex.No: 7  Logic Programming –  Logic Circuit Design
## DATE: 23/09/2024                                                                           
## REGISTER NUMBER : 212222060281
## AIM: 
To write a logic program to design a circuit like half adder, half subtractor, full adder and full subtractor.
##  Algorithm:
1. Start the Program
2. Design a AND gate logic if both inputs are 1 then output is 1.
3. Design a OR gate logic if any one of input is 1 then output is 1.
4. Design a XOR gate logic if both inputs are different then output is 1.
5. Design a NOT gate logic if input is 0 then output is 1.
6. Design a half adder and half subtractor using the rules.
7. Test the logic.
8. Stop the program.

## Program:
```
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

```
### Output:

![image](https://github.com/user-attachments/assets/889e60d1-e9e4-4124-a9de-1654b10d80b2)
![image](https://github.com/user-attachments/assets/74c9a192-6e2d-4d1c-aea5-28e82348c8f4)
![image](https://github.com/user-attachments/assets/143ec4d8-6ce0-4a97-aaae-623cfed5b958)
![image](https://github.com/user-attachments/assets/5cf058c8-da23-40c5-8e5a-d7f377c50a6c)



### Result:
Thus the truth table of circuit verified sucessfully.
