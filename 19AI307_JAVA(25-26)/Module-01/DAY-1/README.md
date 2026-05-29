# Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS

## QUESTION:
Lovely is given a power level before entering a challenge room. She receives 3 bonus potions (each adds +1 using ++) She also steps on 2 traps (each reduces -1 using --). But she doesn't want any logic or loops—just a step-by-step manual update of her power.
Write a program that:
1. Accepts her initial power level.
2. Increases it 3 times using ++.
3. Decreases it 2 times using --.
4. Displays the power level after each step.
5. Finally prints her final power level.

## AIM:
To read two integer values and display the results of various relational operations between them.
## ALGORITHM :
1.	Import the required packages.
2. Create a Scanner object to read input from the user.
3. Declare two integer variables a and b.
4. Read the value of a.
5. Read the value of b.
6. Check whether a is equal to b using == and display the result.
7. Check whether a is not equal to b using != and display the result.
8. Check whether a is greater than b using > and display the result.
9. Check whether a is less than b using < and display the result.
10. Check whether a is greater than or equal to b using >= and display the result.
11. Check whether a is less than or equal to b using <= and display the result.

## PROGRAM:
 ```
/*
Program to implement variables and Operators using Java
Developed by: Vishwaraj G
RegisterNumber:  212223220125
*/
```

## Sourcecode.java:
```java
import java.util.*;
public class Main{
    public static void main(String[] args){
        int a,b;
        Scanner sc = new Scanner(System.in);
        a = sc.nextInt();
        b = sc.nextInt();
        System.out.println("a == b: "+(a==b));
        System.out.println("a != b: "+(a!=b));
        System.out.println("a > b: "+(a>b));
        System.out.println("a < b: "+(a<b));
        System.out.println("a >= b: "+(a>=b));
        System.out.println("a <= b: "+(a<=b));
    }
}
```
## OUTPUT:
![alt text](image.png)


## RESULT:
Thus, the program to perform and display the results of relational operations (==, !=, >, <, >=, <=) between two integers was implemented and executed successfully.