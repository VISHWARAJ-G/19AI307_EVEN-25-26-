# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
A train company charges tickets based on age and travel class: 
1. Children (<12): ₹5 per km (any class)
2. Adults (12–60):
3. Sleeper: ₹10/km
4. AC: ₹15/km
5. Seniors (>60): ₹7/km (any class)
Task: Accept age, distance and travel class (1 for Sleeper, 2 for AC)(follow the same order to get the inputs). Calculate fare.

## AIM:
To calculate the train ticket fare based on the passenger's age, travel distance, and travel class.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a Scanner object to read input from the user.
4. Declare integer variables age and distance.
5. Read the values of age and distance.
6. Check if age is less than 12.
7. If true, calculate fare as distance × 5 and display it.
8. Otherwise, check if age is between 12 and 60 (inclusive).
9. If true, read the value of travelClass.
10. If travelClass is 1, calculate fare as distance × 10. 
11. Otherwise, calculate fare as distance × 15.
12. Display the calculated fare.
13. If age is greater than 60, calculate fare as distance × 7 and display it.
14. End



## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: Vishwaraj G
RegisterNumber:  212223220125
*/
```

## SOURCE CODE:
```java
import java.util.*;
public class Main{
    public static void main(String[] args){
        int age,distance;
        Scanner sc = new Scanner(System.in);
        age = sc.nextInt();
        distance = sc.nextInt();
        if(age<12) System.out.println(distance*5);
        else if(age>=12 && age<=60){
            int travelClass = sc.nextInt();
            System.out.println(travelClass==1?distance*10:distance*15);
        } else System.out.println(distance*7);
    }
}
```






## OUTPUT:

![alt text](image.png)

## RESULT:
Thus, the program to calculate the train ticket fare based on the passenger's age, travel distance, and travel class was implemented and executed successfully.