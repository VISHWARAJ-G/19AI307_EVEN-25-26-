# Ex.No:1(D) ARRAYS

## QUESTION:
Write a Java program to check if an element is present more than once in an array

## AIM:
To check whether an element is present more than once in an array.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a Scanner object to read input from the user.
4. Declare variables range, i, and a boolean variable isRepeated and initialize it to false.
5. Read the value of range.
6. Create an integer array of size range + 1.
7. Read the array elements and store them in the array.
8. Use an outer loop to traverse the array from the first element to the second-last element.
9. Use an inner loop to compare the current element with all subsequent elements.
10. If two elements are found equal, set isRepeated to true and terminate the inner loop.
11. If isRepeated becomes true, terminate the outer loop.
12. Check the value of isRepeated.
13. If true, display "Yes".
14. Otherwise, display "No".
15. End

## PROGRAM:
 ```
/*
Program to implement a Array concept using Java
Developed by: Vishwaraj G
RegisterNumber:  212223220125
*/
```

## SOURCE CODE:
```java
import java.util.*;
public class Main{
    public static void main(String[] args){
        int range,i;
        boolean isRepeated=false;
        Scanner sc = new Scanner(System.in);
        range = sc.nextInt();
        int[] arr = new int[range+1];
        for(i=0;i<=range;i++){
            arr[i] = sc.nextInt();
        }
        for(i=0;i<arr.length-1;i++){
            for(int j=i+1;j<arr.length;j++){
                if(arr[i]==arr[j]){
                    isRepeated = true;
                    break;
                }
            }
            if(isRepeated) break;
        }
        System.out.println(isRepeated?"Yes":"No");
    }
}
```
## OUTPUT:

![alt text](image.png)

## RESULT:
Thus, the program to check whether any element is present more than once in an array was implemented and executed successfully.