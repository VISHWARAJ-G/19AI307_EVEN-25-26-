# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION:
Define class Game with: Static variable maxScore = 500 Print max score via 3 different object references. Change via one object into 800, and print the output of previous maxScore and changed maxScore. 

## AIM:
To demonstrate the behavior of a static variable by accessing and modifying it through multiple object references.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Define a class Game.
4. Declare a static variable maxScore and initialize it to 500.
5. Define the main() method.
6. Create the first object obj1 of the Game class.
7. Display the value of maxScore using obj1.
8. Create the second object obj2 of the Game class.
9. Display the value of maxScore using obj2.
10. Create the third object obj3 of the Game class.
11. Display the value of maxScore using obj3.
12. Modify maxScore to 800 using obj1.
13. Display the updated value of maxScore using obj1.
14. Display the updated value of maxScore using obj2.
15. Display the updated value of maxScore using obj3.
16. Observe that the change is reflected through all object references since maxScore is static.
17. End


## PROGRAM:
 ```
/*
Program to implement a Access Modifiers using Java
Developed by: Vishwaraj G
RegisterNumber: 212223220125
*/
```

## SOURCE CODE:

```java
class Game {
    static int maxScore = 500;
}

class prog {
    public static void main(String[] args){
        Game obj1 = new Game();
        System.out.println(obj1.maxScore);
        Game obj2 = new Game();
        System.out.println(obj2.maxScore);
        Game obj3 = new Game();
        System.out.println(obj3.maxScore);
        obj1.maxScore = 800;
        System.out.println(obj1.maxScore);
        System.out.println(obj2.maxScore);
        System.out.println(obj3.maxScore);
    }
}
```





## OUTPUT:
![alt text](image.png)


## RESULT:
Thus, the program to demonstrate the behavior of a static variable using multiple object references was implemented and executed successfully. It was observed that changing the static variable through one object updated the value for all objects of the class.