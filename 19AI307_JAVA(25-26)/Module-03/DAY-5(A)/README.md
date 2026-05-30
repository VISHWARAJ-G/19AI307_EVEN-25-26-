# Ex.No:3(E) INNER CLASS

## QUESTION:
Write a Java program where the inner class is declared private and accessed through a method in the outer class.

## AIM:
To demonstrate a private inner class and access its data through a public method of the outer class.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Define an outer class OuterClass.
3. Declare a private inner class PrivateInnerClass inside OuterClass.
3. Declare a private integer variable num in the inner class.
3. Define a private method method(int num) to assign a value to num.
3. Define a private method returnNum() to return the value of num.
3. Define a public method accessMethod(int num) in the outer class.
3. Create an object of PrivateInnerClass inside accessMethod().
3. Invoke the method() of the inner class to set the value.
3. Invoke the returnNum() method and return the value.
3. Define the main() method.
3. Create a Scanner object to read input from the user.
3. Read an integer value.
3. Create an object of OuterClass.
3. Call the accessMethod() using the outer class object.
3. Display the value returned from the private inner class.
3. End





## PROGRAM:
 ```
/*
Program to implement a InnerClass using Java
Developed by: Vishwaraj G
RegisterNumber: 212223220125
*/
```

## SOURCE CODE:
```java
import java.util.Scanner;
class OuterClass{
    private class PrivateInnerClass{
        private int num;
        private void method(int num){
            this.num = num;
        }
        private int returnNum(){
            return num;
        }
    }
    public int accessMethod(int num){
        PrivateInnerClass obj = new PrivateInnerClass();
        obj.method(num);
        return obj.returnNum();
    }
}
public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        OuterClass obj = new OuterClass();
        System.out.println("Data set inside private inner class: "+obj.accessMethod(num));
    }
}
```

## OUTPUT:
![alt text](image.png)

## RESULT:
Thus, the program to declare a private inner class and access its members through a method in the outer class was implemented and executed successfully.