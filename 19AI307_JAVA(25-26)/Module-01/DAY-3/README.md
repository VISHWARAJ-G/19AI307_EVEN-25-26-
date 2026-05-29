# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:

Write a Java program that prompts the user to enter the number of rows (or size) of the square and prints a hollow square pattern of that size.

- Use nested for loops to generate the pattern.

- Print stars (*) for the first and last rows, and for the first and last columns of each row.

- Leave spaces in all other positions to create the hollow effect.

## AIM:
To print a hollow square pattern of a given size using nested for loops.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a Scanner object to read input from the user.
4. Declare an integer variable row.
5. Read the value of row.
6. Use an outer loop to iterate through each row from 0 to row - 1.
7. Use an inner loop to iterate through each column from 0 to row - 1.
8. Check if the current position belongs to the first row, last row, first column, or last column.
9. If true, print "* ".
10. Otherwise, print two spaces " ".
11. After completing each row, move to the next line.
12. Repeat until all rows are printed.
13. End


## PROGRAM:
 ```
/*
Program to implement a Looping Statement using Java
Developed by: Vishwaraj G
RegisterNumber:  212223220125
*/
```

## SOURCE CODE:
```java
import java.util.*;
public class Main{
    public static void main(String[] args){
        int row;
        Scanner sc=new Scanner(System.in);
        row = sc.nextInt();
        for(int i=0;i<row;i++){
            for(int j=0;j<row;j++){
                if(i==0||i==row-1||j==0||j==row-1)
                    System.out.print("* ");
                else
                    System.out.print("  ");
            }
            System.out.println();
        }
    }
}
```






## OUTPUT:

![alt text](image.png)

## RESULT:
Thus, the program to print a hollow square pattern of the given size using nested for loops was implemented and executed successfully.