# Preferred Population Health Management
## Interview Tech Test (Answers)


## Answer 1

Somthing like this:

```csharp
static long TotalAllEvenNumbers(int[] intArray) {
  return intArray.Where(i => i % 2 == 0).Sum(i => (long)i);
}
```

or like this:

```csharp
static long TotalAllEvenNumbers(int[] intArray) {
  return (from i in intArray where i % 2 == 0 select (long)i).Sum();
}
```


### Key things to look for:
+ Does the candidate take advantage of the C# language constructs which make a one-liner solution possible (i.e., rather than employing a more lengthy solution which contains a loop, conditional statement, and accumulator)?

+ Does the candidate consider the possibility of overflow. For example, an implementation such as ```return intArray.Where(i => i % 2 == 0).Sum()``` (regardless of the return type of the function) might be an “obvious” one-line solution, but the probability of overflow here is high. While the approach used in the answers above of converting to long doesn’t eliminate the possibility, it makes it a highly unlikely that an overflow exception will occur. Note that, if the candidate asks about the expected size of the array and the magnitude of its members, he or she is obviously considering this overflow issue, which is part of what we’re looking to ascertain.
#

## Answer 2

The output will be:

```csharp
location is null
1/1/0001 12:00:00 AM
```

Although both variables are uninitialized, `String` is a reference type and `DateTime` is a value type. As a value type, an unitialized `DateTime` variable is set to a default value of midnight of 1/1/1 (yup, that’s the year 1 A.D.), not `null`.
#

## Answer 3
One might think that, since a `DateTime` variable can never be null (it is automatically initialized to Jan 1, 0001), the compiler would complain when a `DateTime` variable is compared to `null`. However, due to type coercion, the compiler does allow it, which can potentially lead to headfakes and pull-out-your-hair bugs.

Specifically, the `==` operator will cast its operands to different allowable types in order to get a common type on both sides, which it can then compare. That is why something like this will give you the result you expect (as opposed to failing or behaving unexpectedly because the operands are of different types):

```csharp
double x = 5.0;
int y = 5;
Console.WriteLine(x == y);  // outputs true
```

However, this can sometimes result in unexpected behavior, as is the case with the comparison of a `DateTime` variable and `null`. In such a case, both the `DateTime` variable and the `null` literal can be cast to `Nullable<DateTime>`. Therefore it is legal to compare the two values, even though the result will always be false.
#

## Answer 4

Yes! It is possible to do so because the array can be of type object that can not only store any datatype but also the object of the class as shown below:
#

## Answer 5
This can be achieved using `String.Replace()` method on the string in question, in conjucntion with a regex statement.
#

## Answer 6

`TestValue : 10`

The static constructor of a class is called before any instance of the class is created. The static constructor called here initializes the `TestValue` variable first.
#

## Answer 7

Dependency injection is a way to de-couple tightly linked classes, thereby reducing the direct dependency of classes upon each other. There are different ways by which dependency injection can be achived:

+ Constructor dependency
+ Property dependency
+ Method dependency
#

## Answer 8

Something like this:

```csharp
using system;
class abc
{
    public static Void Main()
    {
        int ndistance, nresult;
        Console.WriteLine("Enter the distance in kilometers");
        ndistance = convert.ToInt32(Console.ReadLine());
        nresult = ndistance * 1000;
        Console.WriteLine("Distance in meters: " + nresult);
        Console.ReadLine();
    }
}
```
#

## Answer 9

The answer is C
#

## Answer 10

The answer is C
#

## Answer 11
The answer is:
```csharp
    first method
    10
    first method
    second method
```
#

## Answer 12

The answer is A

#

## Answer 13

The answer is B

#

## Answer 14

The answer is C

#

## Answer 15

The answer is: `Akshay is in city new delhi`

#


