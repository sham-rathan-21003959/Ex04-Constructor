# Ex04-Constructor
## Aim:
 To write a C# program to calculate the salary of an employee by passing the name, designation, noofexperience, basic salary and insurance amount through constructor.
 
## Algorithm:
### Step 1:
Start the C# program in visual studio 2022.
### Step 2:
Create a class and a constructor.
### Step 3:
Get employee name, Designation, No of experience, basic salary and insurance amount from the User.
### Step 4:
Call salary method in constructor to calculate salary.
### Step 5:
Call display method to display the output.
### Step 6:
Stop the C# program and Run the prgram.
### Step 7:
Take the screenshot of the output.
### Step 8:
Close.
 
## Program:
```
Developed by: SHAM RATHAN S
Register no : 212221230093

using System;
public class Employee
{
    public String designation;
    public String employee_name;
    public int exp;
    public int bs;
    public int insurance;
    double hra, ta, salary;

    public Employee(String employee_name, String designation, int exp, int bs, int i)
    {
        this.employee_name = employee_name;
        this.designation = designation;
        this.exp = exp;
        this.bs = bs;
        this.insurance = i;
    }
    public void sal()
    {
        hra = this.bs * 0.2;
        ta = this.bs * 0.1;
        salary = this.bs + hra + ta - this.insurance;

    }
    public void display()
    {

        Console.WriteLine("Name of the employee is {0} having {1} of experience,working as {2}", this.employee_name, this.exp, this.designation);
        Console.WriteLine("Receives {0} of salary.", salary);

    }

}
class TestEmployee
{
    public static void Main(string[] args)
    {
        Employee e1 = new Employee("Shankar", "Teacher", 8, 30000, 1000);
        e1.sal();
        Employee e2 = new Employee("Reshma", "Vice principal", 5, 45000, 3000);
        e2.sal();
        e1.display();
        e2.display();

    }
}
```
 
## Output:
![out](https://user-images.githubusercontent.com/93587823/190552571-1aff1335-b776-42b9-a9ac-51a7fad9fb9b.png)
 
## Result:
Thus C# program to calculate the salary of an employee by passing the name, designation, noofexperience, basic salary and insurance amount through constructor is executed successfully.
