# Ex.No: 6   Towers of Hanoi _ Prolog 
### DATE:  9/09/2024                                                                          
### REGISTER NUMBER : 212222040091
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

![Screenshot 2024-10-07 093716](https://github.com/user-attachments/assets/4d1122c3-1416-41bd-a6b7-91a2b1201f6a)


![Screenshot 2024-10-07 093742](https://github.com/user-attachments/assets/2dc314c7-ee10-4ff9-b89c-f0b22927575e)



### Result:
Thus the solution of Towers of Hanoi problem was found by logic programming.
