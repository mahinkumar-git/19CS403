# Ex.No:4(D) DESIGN PATTERN  ---- BEHAVIOUR PATTERN

## QUESTION:
Create an MVC program for a School System where the DAO stores student info, controller fetches it, and view displays it.

For example:

Input	Result
3
Siva
18
IT100
Karthik
19
IT101
Ramya
20
IT102
IT102
Student Details:
Name    : Ramya
Age     : 20
Roll No : IT102
4
Rahul
22
EEE001
Preethi
23
EEE002
Naveen
21
EEE003
Divya
20
EEE004
EEE003
Student Details:
Name    : Naveen
Age     : 21
Roll No : EEE003



## AIM:

To develop a Java program using the MVC (Model–View–Controller) architecture, where the DAO stores student information, the Controller fetches the data, and the View displays the student details.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a Model (Student) class with name, age, and roll number.
4.	Create DAO interface with methods to add and get student.
5.	Implement DAO using a list to store student objects.
6.	Create a View class to display student details.
7.	Create a Controller class to interact with DAO and View.
8.	Read number of students and their details from input.
9.	Add each student to DAO through Controller.
10.	Read the roll number to search.
11.	Controller fetches the student from DAO and View displays it.
12.	End program.
   





## PROGRAM:
 ```
/*
Program to implement a Behaviour Pattern using Java
Developed by: Mahinkumar T.
RegisterNumber: 212222040094
*/
```

## SOURCE CODE:


```
import java.util.*;

// Model
class Student {
    private String name;
    private int age;
    private String rollNo;

    public Student(String name, int age, String rollNo) {
        this.name = name;
        this.age = age;
        this.rollNo = rollNo;
    }

    public String getName() { return name; }
    public int getAge() { return age; }
    public String getRollNo() { return rollNo; }
}

// DAO Interface
interface StudentDAO {
    void addStudent(Student student);
    Student getStudentByRollNo(String rollNo);
}

// DAO Implementation
class StudentDAOImpl implements StudentDAO {
    private List<Student> students = new ArrayList<>();

    public void addStudent(Student student) {
        students.add(student);
    }

    public Student getStudentByRollNo(String rollNo) {
        for (Student s : students) {
            if (s.getRollNo().equals(rollNo)) {
                return s;
            }
        }
        return null;
    }
}

// View
class StudentView {
    public void displayStudent(Student student) {
        if (student != null) {
            System.out.println("Student Details:");
            System.out.println("Name    : " + student.getName());
            System.out.println("Age     : " + student.getAge());
            System.out.println("Roll No : " + student.getRollNo());
        } else {
            System.out.println("Student not found.");
        }
    }
}

// Controller
class StudentController {
    private StudentDAO dao;
    private StudentView view;

    public StudentController(StudentDAO dao, StudentView view) {
        this.dao = dao;
        this.view = view;
    }

    public void addStudent(Student student) {
        dao.addStudent(student);
    }

    public void showStudent(String rollNo) {
        Student student = dao.getStudentByRollNo(rollNo);
        view.displayStudent(student);
    }
}

// Main class
public class SchoolSystemMVC {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        StudentDAO dao = new StudentDAOImpl();
        StudentView view = new StudentView();
        StudentController controller = new StudentController(dao, view);

        int n = sc.nextInt();
        sc.nextLine();
        for (int i = 0; i < n; i++) {
            String name = sc.nextLine();
            int age = sc.nextInt();
            sc.nextLine();
            String rollNo = sc.nextLine();
            controller.addStudent(new Student(name, age, rollNo));
        }

        String searchRollNo = sc.nextLine();
        controller.showStudent(searchRollNo);
        sc.close();
    }
}

```



## OUTPUT:

<img width="664" height="865" alt="image" src="https://github.com/user-attachments/assets/513d52e2-81c4-4919-9d33-d323187348ed" />


## RESULT:

Thus, a School System was successfully implemented using the MVC architecture, where the DAO stores student data, the Controller retrieves it, and the View displays it.
