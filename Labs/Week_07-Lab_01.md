# การทดลองที่ 7.1

1. ให้สร้าง project เป็น console application และรันโค้ดต่อไปนี้

``` c#
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Week7_Lab1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            var person1 = new Person();
            person1.Name = "Rambo";
            person1.Age = 25;
            person1.TellAge();
            person1.TellName();
        }
    }
    class Person
    { 
        // Fields
        private string name;
        private int age;

        // Properties
        public string Name
        {
            get { return name; }
            set { name = value; }
        }

        public int Age
        {
            get { return age; }
            set { age = value; }
        }

        // Methods
        public void TellAge()
        {
            Console.WriteLine($"My age is {age}");
        }
        public void TellName()
        {
            Console.WriteLine($"My name is {name}");
        }

    }
}

```


### บันทึกผล




---

# Assignment
## 1. ให้เขียนโปรแกรมโดยใช้โปรแกรมด้านบนเป็นตัวอย่าง 

### 1.1 สร้างคลาส `Student` โดยมี members ดังต่อไปนี้


|Member type|     name   |data type|modifier | Accessor |
|:---------:|:----------:|:-------:|:-------:|:--------:|
|field      | studentID  | string  | private |          |
|field      | name       | string  | private |          |
|field      | age        | int     | private |          |
|field      | major      | string  | private |          |
|field      | school     | string  | private |          |
|field      | gpa        | float   | private |          |
|property   | StudentID  | string  | public  | getter, setter |
|property   | Name       | string  | public  | getter, setter |
|property   | Age        | int     | public  | getter, setter |
|property   | Major      | string  | public  | getter, setter |
|property   | School     | string  | public  | getter, setter |
|property   | GPA        | float   | public  | getter, setter |
|Method     | TellStudentID()     | void    | public  | |
|Method     | TellName()     | void    | public  | |
|Method     | TellAge()     | void    | public  | |
|Method     | TellMajor()     | void    | public  | |
|Method     | TellSchool()     | void    | public  | |
|Method     | TellGPA()     | void    | public  | |


### 1.2  ทดสอบโดยเขียน Code ใน Main() ดังต่อไปนี้

```cs
static void Main(string[] args)
{
    var student1 = new Student();
    student1.Name = "ชื่อของนักศึกษาเอง";
    student1.Age = อายุ;
    // ..... เขียนให้ครบทุก properties

    // เรียกใช้งานวัตถุ
    student1.TellName();
    // ..... เรียกใช้ให้ครบทุก method
}
```

### บันทึกผล
