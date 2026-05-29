# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a Java program to remove all spaces from a given string.

## AIM:
To remove all spaces from a given string and display the modified string.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a Scanner object to read input from the user.
4. Read the input string and store it in a StringBuilder object str.
5. Create an empty StringBuilder object newStr.
6. Traverse each character of the string using a loop.
7. Check whether the current character is a space.
8. If the character is not a space, append it to newStr.
9. Repeat the process until all characters are checked.
Display the string stored in newStr.
10. End

## PROGRAM:
 ```
/*
Program to implement a Strings and Math Function using Java
Developed by: Vishwaraj G
RegisterNumber:  212223220125
*/
```

## SOURCE CODE:
```java
import java.util.Scanner;
public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        StringBuilder str = new StringBuilder(sc.nextLine());
        StringBuilder newStr = new StringBuilder();
        for(int i=0;i<str.length();i++){
            if(str.charAt(i)!=' ')
                newStr.append(str.charAt(i));
        }
        System.out.println("String without spaces: "+newStr);
    }
}
```






## OUTPUT:

![alt text](image.png)

## RESULT:
Thus, the program to remove all spaces from a given string and display the modified string was implemented and executed successfully.