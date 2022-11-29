# Inheritance

## Aim:
To write a C# program to print some messages using hierarchical inheritance



## Algorithm:
Step 1:Create a base class.
Step 2:Create two child class.
Step 3:Create a constructor in the base class and print a message.
Step 4:Create a function in child class to print a message.


## Program:
~~~
using System;
namespace Autovechicle
{
    public class tyre
    {
        public tyre()
        {
            Console.WriteLine("Constructor tyre");
        }
        public virtual void Display()
        {
            Console.WriteLine("tyre");
        }
    }
    public class scooter : tyre
    {
        public scooter()
        {
            Console.WriteLine("Constructor sports car");
        }

        public override void Display()
        {
            base.Display();
            Console.WriteLine("sports car");
        }
    }
    public class car : tyre
    {
        public car()
        {
            Console.WriteLine("Constructor bike");
        }
        public override void Display()
        {
            base.Display();
            Console.WriteLine("bike");
        }
    }
    public class Program
    {
        public static void Main(string[] args)
        {
            car cd = new car();
            scooter cdd = new scooter();
            cd.Display();
            cdd.Display();
        }
    }
}
~~~


## Output:
![image](https://user-images.githubusercontent.com/94187572/204549457-712cd945-fbb9-49f3-9e0b-27d7317e241c.png)



## Result
C# program to print some messages using hierarchical inheritance is implemented successfully.


