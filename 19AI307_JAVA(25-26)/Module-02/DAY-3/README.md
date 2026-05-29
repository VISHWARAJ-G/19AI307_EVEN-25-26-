# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:
Write a Java program to create a class called Rectangle with private instance variables length and width. Provide public getter and setter methods to access and modify these variables
## AIM:
To create a class Rectangle with private instance variables length and width, and provide public getter and setter methods to access and modify these variables.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3. Define a class Rectangle.
4. Declare private instance variables length and width.
5. Create a public method getLength() to return the value of length.
6. Create a public method setLength() to assign a value to length.
7. Create a public method getWidth() to return the value of width.
8. Create a public method setWidth() to assign a value to width.
9. Create a method calculateArea() to compute the area of the rectangle.
10. Define the main() method.
11. Create a Scanner object to read input from the user.
12. Create an object of the Rectangle class.
13. Read the length value and set it using setLength().
14. Read the width value and set it using setWidth().
15. Retrieve the length using getLength() and display it.
16. Retrieve the width using getWidth() and display it.
17. End





## PROGRAM:
 ```
/*
Program to implement a Access Specifiers using Java
Developed by: Vishwaraj G
RegisterNumber:  212223220125
*/
```

## SOURCE CODE:
```java
import java.util.Scanner;
class Rectangle {
    private double length;
    private double width;
    public double getLength() {
        return length;
    }
    public void setLength(double length) {
        this.length = length;
    }
    public double getWidth() {
        return width;
    }
    public void setWidth(double width) {
        this.width = width;
    }
    public double calculateArea() {
        return length * width;
    }
}
public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        Rectangle rectObj = new Rectangle();
        rectObj.setLength(sc.nextDouble());
        rectObj.setWidth(sc.nextDouble());
        System.out.println("Length: "+rectObj.getLength());
        System.out.println("Width: "+rectObj.getWidth());
    }
}
```






## OUTPUT:
![alt text](image.png)


## RESULT:
Thus, the program to create a Rectangle class with private instance variables and public getter and setter methods was implemented and executed successfully.