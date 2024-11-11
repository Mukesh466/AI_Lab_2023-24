# Ex.No: 6   Logic Programming – Towers of Hanoi  
### DATE: 26.09.2024                                                                            
### REGISTER NUMBER : 212223060174
### AIM: 
To  write  a logic program  to solve Towers of Hanoi problem  using SWI-PROLOG. 
### Algorithm:
1. Start the program
2.  Write a rules for finding solution of Towers of Hanoi in SWI-PROLOG.
3.  a )	If only one disk  => Move disk from X to Y.
4.  b)	If Number of disk greater than 0 then
5.        i)	Move  N-1 disks from X to Z.
6.        ii)	Move  Nth disk from X to Y
7.        iii)	Move  N-1 disks from Y to X.
8. Run the program  to find answer of  query.

### Program:
```
move(1,X,Y,_) :-  
    write('Move top disk from '), 
    write(X), 
    write(' to '), 
    write(Y), 
    nl. 
move(N,X,Y,Z) :- 
    N>1, 
    M is N-1, 
    move(M,X,Z,Y), 
    move(1,X,Y,_), 
    move(M,Z,Y,X).
```



### Output:
![Screenshot 2024-03-29 225802](https://github.com/Vikhram-S/AI_Lab_2023-24/assets/146576573/0fbb8cd4-a493-411e-b5c1-cd83820bd3d7)




### Result:
Thus the solution of Towers of Hanoi problem was found by logic programming.
