# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:
Define a class Teacher with attributes: name (String), subject (String), and experience (int, years). 



## AIM:
To define a Java class Teacher with attributes name, subject, and experience.

## ALGORITHM :
1.	Create a class named Teacher.
2.	Declare attributes name, subject, and experience.
3.	Define a constructor to initialize these attributes.
4.	Add a method displayDetails() to print teacher details.
5.	End the program.





## PROGRAM:
 ```
/*
Program to implement a Class and Objects using Java
Developed by: Mahinkumar T.
RegisterNumber: 212222040094
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Teacher {
    String name;
    String subject;
    int experience;

    void printMessage() {
        System.out.print("Mr. " + name + " teaches " + subject + " and has " + experience + " years experience.");
    }
}

class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Teacher t = new Teacher();
        t.name = sc.nextLine();
        t.subject = sc.nextLine();
        t.experience = sc.nextInt();

        t.printMessage();
    }
}

```





## OUTPUT:
<img width="1242" height="426" alt="image" src="https://github.com/user-attachments/assets/46eae97c-9961-4dff-8ce5-ba60ddcf24f6" />



## RESULT:
The Teacher class is successfully defined with the required attributes and methods.


