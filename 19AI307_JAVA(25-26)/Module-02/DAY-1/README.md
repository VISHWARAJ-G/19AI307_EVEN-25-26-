# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:
Define a class Teacher with attributes: name (String), subject (String), and experience (int, years). 

## AIM:
To create a class Teacher with attributes name, subject, and experience, and display the teacher's details using a member function.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Define a class Teacher.
4. Declare the attributes name, subject, and experience.
5. Define a method printMessage() to display the teacher's details.
6. Define the main class prog.
7. Create a Scanner object to read input from the user.
8. Create an object of the Teacher class.
9. Read the teacher's name and store it in name.
10. Read the subject and store it in subject.
11. Read the years of experience and store it in experience.
12. Invoke the printMessage() method using the object.
Display the teacher's name, subject, and experience.
13. End

## PROGRAM:
 ```
/*
Program to implement a Class and Objects using Java
Developed by: Vishwaraj G
RegisterNumber:  212223220125
*/
```

## SOURCE CODE:
```java
import java.util.Scanner;
class Teacher {
    String name;
    String subject;
    int experience;

    void printMessage() {
        System.out.println("Mr. "+name+" teaches "+subject+" and has "+experience+" years experience.");
    }
}
class prog {
    public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
       Teacher obj = new Teacher();
       obj.name = sc.next();
       obj.subject = sc.next();
       obj.experience = sc.nextInt();
       obj.printMessage();
    }
}
```






## OUTPUT:

![alt text](image.png)

## RESULT:
Thus, the program to create a Teacher class with attributes name, subject, and experience, and display the teacher's details using a method was implemented and executed successfully.