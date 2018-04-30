# Preferred Population Health Management
## Interview Tech Test (Written)

## Instructions: 

This tech test is used to test the fundamental skills used to program in C# and .NET. There will be a mixture of multiple choice and written answer questions throughout the test. The internet may not be utilized for this test due to the fact of its fundamental nature. You should be able to get through all of these questions without having to rely on the interet. We also don't want you looking at the internet because we want to see how you think individually. Good luck.

### Q1: Given an array of ints, write a method to total all the values that are even numbers.
#
#
#
#
#
#
#
### Q2: What is the output of the code below? Explain your answer.

```csharp
class Program {
  static String location;
  static DateTime time;
 
  static void Main() {
    Console.WriteLine(location == null ? "location is null" : location);
    Console.WriteLine(time == null ? "time is null" : time.ToString());
  }
}
```
### Answer:
#
#
#
#
#
#

### Q3: Is the comparison of time and null in the if statement below valid or not? Why or why not?

```csharp
static DateTime time;

if (time == null)
{
	/* do something */
}
```
### Answer:
#
#
#
#
#
#

### Q4: It is possible to store mixed datatypes such as int, string, float, char all in one array? Explain your answer.
### Answer:
#
#
#
#
#
#

### Q5: You’re given a word string containing one or many $ symbols, e.g.:
```csharp
string example = "foo bar foo $ bar $ foo bar $ "
```
### Question: How do you remove the second and third occurrences of $ from a given string?
### Answer:
#
#
#
#

### Q6: What is the output of the program below?
```csharp
public class TestStatic
{
    public static int TestValue;

    public TestStatic()
    {
        if (TestValue == 0)
            TestValue = 5;
    }
    static TestStatic()
    {
        if (TestValue == 0)
            TestValue = 10;
    }

    public void Print()
    {
        if (TestValue == 5)
            TestValue = 6;                

        Console.WriteLine("TestValue : " + TestValue);
    } 
}

public void Main(string[] args)
{
    TestStatic t = new TestStatic();
    t.Print();
}
```
### Answer:
#
#
#

### Q7: Describe dependency injection.
### Answer:
#
#
#
#
#
#
#
#

### Q8: Write out a C# program that accepts a distance in kilometers, converts it into meters, and then displays the result.
### Answer:
#
#
#
#
#
#
#
#
#

### Q9: Which of the following operators can be used to access the member function of a class? (Circle Answer)
- A) :
- B) ::
- C) .
- D) #

### Q10: Which of the following statements are correct for the given code snippet? (Circle Answer)
```csharp
shape obj;
obj = new shape();
```

- A) Creates an object of class shape.
- B) To create an object of type shape on the heap or stack depending on size.
- C) Creates a reference object to class shape and an object of type shape on the heap.
- D) Create an object of type shape on the stack.

### Q11: What will be the outcome of the following code snippet?
```csharp
using System;
class sample
{
    public static void first()
    {
        Console.WriteLine("first method");
    }
    public void second()
    {
        first();
        Console.WriteLine("second method");
    }
    public void second(int i)
    {
        Console.WriteLine(i);
        second();
    }
}
class program
{
    public static void Main()
    {
        sample obj = new sample();
        sample.first();
        obj.second(10);
    }
}
```
### Answer:
#
#
#
#
#

### Q12: What will be the output of the following code? (Circle Answer)
```csharp
using System;
class program
{
    static void Main(string[] args)
    {
        int num = 2;
        fun1 (ref num);
        Console.WriteLine(num);
        Console.ReadLine();
    }
    static void fun1(ref int num)
    {
        num = num * num * num;
    }
} 
```
- A) 8
- B) 0
- C) 2
- D) 16

### Q13: What will be the outcome of the following code snippet? (Circle Answer)
```csharp
using System;
class program
{
    static void Main(string[] args)
    { 
        int[] arr = new int[] { 1, 2, 3, 4, 5 };
        fun1(ref arr);
        Console.ReadLine();
    }
    static void fun1(ref int[] array)
    {
        for (int i = 0; i < array.Length; i=i+2)
        {
            array[i] = array[i] + 10;
        }
        Console.WriteLine(string.Join(",", array));
    }
} 
```
- A) 1 2 3 4 5
- B) 11 2 13 4 15
- C) 11 12 13 14 15
- D) 1 3 5 7 9

### Q14: What will be the outcome of the following code snippet? (Circle Answer)
```csharp
using System;
class program
{
   static void Main(string[] args)
    {
        int x = 4 ,b = 2;
        x -= b/= x * b;
        Console.WriteLine(x + " " + b);
        Console.ReadLine();
    } 
}
```

- A) 4 2
- B) 0 4
- C) 4 0
- D) Not mentioned

### Q15: What will be the outcome of the following code snippet?
```csharp
using System;
class emp
{
    public string name;
    public string address;
    public void display()
    {
        Console.WriteLine("{0} is in city {1}", name, address);
    }
}
class Program
{
    static void Main(string[] args)
    {
        emp obj = new emp();
        obj.name = "Akshay";
        obj.address = "new delhi";
        obj.display();
        Console.ReadLine();
    }
}
```
### Answer:
#
#
