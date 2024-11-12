# Ex.No: 10  Logic Programming –  Simple queries from facts and rules
### DATE:   19/09/2024                                                                         
### REGISTER NUMBER : 212223060004
### AIM: 
To write a prolog program to find the answer of query. 
###  Algorithm:
 Step 1: Start the program <br> 
 Step 2: Convert the sentence into First order Logic  <br> 
 Step 3:  Convert the sentence into Horn clause form  <br> 
 Step 4: Add rules and predicates in a program   <br> 
 Step 5:  Pass the query to program. <br> 
 Step 6: Prolog interpreter shows the output and return answer. <br> 
 Step 8:  Stop the program.
### Program:
### Task 1:
Construct the FOL representation for the following sentences <br> 
1.	John likes all kinds of food.  <br> 
2.	Apples are food.  <br> 
3.	Chicken is a food.  <br> 
4.	Sue eats everything Bill eats. <br> 
5.	 Bill eats peanuts  <br> 
   Convert into clause form and Prove that John like Apple by using Prolog. <br> 
### Program:
likes(john, X) :- food(X).<br>
food(apple).<br>
food(chicken).<br>
eats(sue, X) :- eats(bill, X).<br>
eats(bill, peanuts).<br>


### Output:
![image](https://github.com/user-attachments/assets/9037b70e-eac2-427a-ab30-b7ead2a2c5df)


### Task 2:
Consider the following facts and represent them in predicate form: <br>              
1.	Steve likes easy courses. <br> 
2.	Science courses are hard. <br> 
3. All the courses in Have fun department are easy <br> 
4. BK301 is Have fun department course.<br> 
Convert the facts in predicate form to clauses and then prove by resolution: “Steve likes BK301 course”<br> 

### Program:
have_fun_course(bk301).<br>
likes(steve, X) :- easy(X).<br>
easy(X) :- have_fun_course(X).<br>

### Output:
![image](https://github.com/user-attachments/assets/1f1dcb9a-3ae0-4269-9c63-2d727bdf44ab)

### Task 3:
Consider the statement <br> 
“This is a crime for an American to sell weapons to hostile nations. <br>
The Nano , enemy of America has some missiles and its missiles were sold it by Colonal West who is an American” <br> 
Convert to Clause form and prove west is criminal by using Prolog.<br> 
### Program:
hostile(nano).<br>
american(west).<br>
missile(missile1).<br>
sells(west, missile1, nano).<br>
criminal(X) :- american(X), sells(X, Y, Z), missile(Y), hostile(Z).<br>

### Output:
![image](https://github.com/user-attachments/assets/6d4ce6a0-594b-4a34-b6a4-28d43efabd61)

### Result:
Thus the prolog programs were executed successfully and the answer of query was found.
