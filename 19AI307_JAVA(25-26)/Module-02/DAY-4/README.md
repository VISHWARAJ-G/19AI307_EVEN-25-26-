# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Write a recursive method that uses a static counter variable and a local variable. Compare how each behaves through recursive calls.

## AIM:
To write a recursive method that demonstrates the behavior of a static counter variable and a local variable through recursive calls.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Define a class Counter.
4. Declare a static variable counter and initialize it to 1.
5. Define a recursive method decrement(int n).
6. Check if n is less than or equal to 0.
7. If true, return from the method.
8. Declare a local variable localCounter and initialize it to 1.
9. Display the current recursive call number.
10. Display the value of the static variable counter.
11. Display the value of the local variable localCounter.
12. Increment the static variable counter.
13. Increment the local variable localCounter.
14. Call the decrement() method recursively with n - 1.
15. In the main() method, create a Scanner object.
16. Read an integer value from the user.
17. Create an object of the Counter class.
18. Invoke the decrement() method with the input value.
19. End





## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: Vishwaraj G
RegisterNumber:  212223220125
*/
```

## SOURCE CODE:
```java

import java.util.Scanner;
class Counter{
    static int counter = 1;
    public int decrement(int n){
        if(n<=0) return 1;
        int localCounter = 1;
        System.out.println("Recursive call "+n);
        System.out.println("Static counter: "+counter);
        System.out.println("Local counter : "+localCounter);
        System.out.println("---------------------------");
        counter++;
        localCounter++;
        return decrement(n-1);
    }
}
public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        Counter ctrObj = new Counter();
        ctrObj.decrement(sc.nextInt());
    }
}
```






## OUTPUT:
![alt text](image.png)



## RESULT:
Thus, the recursive method using a static counter variable and a local variable was implemented and executed successfully. It was observed that the static variable retained its updated value across recursive calls, whereas the local variable was reinitialized during each call.