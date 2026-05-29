# Ex.No:2(B) METHODS

## QUESTION:
Write a method int cube(int x) that calls a method int square(int x) internally to calculate the cube as x * square(x).

## AIM:
To calculate the cube of a number by calling the square() method inside the cube() method.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Define a method square(int x) that returns the square of x.
4. Define a method cube(int x).
5. Inside the cube() method, call the square() method.
6. Calculate the cube as x * square(x).
7. Return the calculated cube value.
8. In the main() method, create a Scanner object.
9. Read an integer value from the user.
10. Call the cube() method with the input value.
11. Display the returned cube value.
12. End

## PROGRAM:
 ```
/*
Program to implement a Methods using Java
Developed by: Vishwaraj G
RegisterNumber:  212223220125
*/
```

## SOURCE CODE:
```java
import java.util.Scanner;
public class Main{
    public static int square(int x){
        return x*x;
    }
    public static int cube(int x){
        return x*square(x);
    }
    public static void main(String[] args){
        int num;
        Scanner sc = new Scanner(System.in);
        num = sc.nextInt();
        System.out.println(cube(num));
    }
}
```






## OUTPUT:
![alt text](image.png)


## RESULT:
Thus, the program to calculate the cube of a number by invoking the square() method within the cube() method was implemented and executed successfully.