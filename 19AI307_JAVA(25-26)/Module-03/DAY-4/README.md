# Ex.No:3(D)    INTERFACE 

## QUESTION:
Schools use different grading schemes. You need to build a system to plug different strategies.

- SimpleGrader: A: 90+, B: 75–89, C: 60–74, F: below 60

- StrictGrader: A: 95+, B: 85–94, C: 70–84, F: below 70

## AIM:
To implement different grading schemes using interfaces and calculate grades based on the selected grading strategy.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Define an interface Grader.
4. Declare the method gradeSystem(int marks) in the interface.
4. Create a class SimpleGrader that implements the Grader interface.
4. Implement the gradeSystem() method with the grading criteria:
    - A: 90 and above
    - B: 75 to 89
    - C: 60 to 74
    - F: below 60
4. Create a class StrictGrader that implements the Grader interface.
4. Implement the gradeSystem() method with the grading criteria:
    - A: 95 and above
    - B: 85 to 94
    - C: 70 to 84
    - F: below 70
4. Define the main() method.
4. Create a Scanner object to read input from the user.
4. Read the student's marks.
4. Read the grading scheme choice.
4. Declare a reference variable of type Grader.
4. If the choice is 1, create an object of SimpleGrader.
4. Invoke the gradeSystem() method and display the grade.
4. If the choice is 2, create an object of StrictGrader.
4. Invoke the gradeSystem() method and display the grade.
4. Terminate the program.

4. End





## PROGRAM:
 ```
/*
Program to implement a Interface using Java
Developed by: Vishwaraj G
RegisterNumber: 212223220125
*/
```

## SOURCE CODE:
```java
import java.util.Scanner;
interface Grader{
    void gradeSystem(int marks);
}
class SimpleGrader implements Grader{
    public void gradeSystem(int marks){
        if(marks>=90)
            System.out.println("A");
        else if(marks<90 && marks >= 75)
            System.out.println("B");
        else if(marks<75 && marks >= 60)
            System.out.println("C");
        else 
            System.out.println("F");
    }
}
class StrictGrader implements Grader{
    public void gradeSystem(int marks){
        if(marks>=95)
            System.out.println("A");
        else if(marks<95 && marks >= 85)
            System.out.println("B");
        else if(marks<85 && marks >= 70)
            System.out.println("C");
        else 
            System.out.println("F");
    }
}
public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int grade = sc.nextInt();
        int choice = sc.nextInt();
        Grader grader;
        if(choice==1){
            grader = new SimpleGrader();
            grader.gradeSystem(grade);
        } else if(choice==2){
            grader = new StrictGrader();
            grader.gradeSystem(grade);
        }
    }
}
```






## OUTPUT:
![alt text](image.png)


## RESULT:
Thus, the program to implement multiple grading schemes using interfaces and determine grades based on the selected grading strategy was implemented and executed successfully.