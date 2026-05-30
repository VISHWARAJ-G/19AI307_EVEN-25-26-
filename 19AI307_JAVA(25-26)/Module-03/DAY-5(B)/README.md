# Ex.No:3(F) WRAPPER CLASS

## QUESTION:
Write a Java program to find the square root of a number using Double wrapper class.

## AIM:
To find the square root of a number using the Double wrapper class.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a Scanner object to read input from the user.
4. Declare a Double variable value.
4. Read a double value from the user and store it in value.
4. Calculate the square root of value using the Math.sqrt() method.
4. Display the original number and its square root.
4. Terminate the program.
4. End





## PROGRAM:
 ```
/*
Program to implement a Wrapper Class using Java
Developed by: Vishwaraj G
RegisterNumber: 212223220125
*/
```

## SOURCE CODE:
```java
import java.util.Scanner;
public class Main{
    public static void main(String[] args){
        Double value;
        Scanner sc = new Scanner(System.in);
        value = sc.nextDouble();
        System.out.printf("Square root of %.1f is: %.1f",value,Math.sqrt(value));
    }
}
```






## OUTPUT:
![alt text](image.png)

## RESULT:
Thus, the program to find the square root of a number using the Double wrapper class was implemented and executed successfully.