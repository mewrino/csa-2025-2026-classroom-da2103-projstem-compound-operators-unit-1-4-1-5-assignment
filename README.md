# unit-1-4-1-5-assignment

## Order of Operations Practice
**Instructions:** Evaluate the following expressions.  You can answer either in this README file, in your own notebook, or on a separate piece of paper.
### Part 1
a. 3 * (7 - 4) + 6 / 2

b. ((12 / 3) * (7 - 5) + 4) / 2

c. (5 + 2) * (8 - 3) % 2

d. (15 % 4) + (5 / 2) - (3 * 2)

e. 5 * 2 + 4 / 2 % 3

f. (18 - 12) % 3 * (5 - 3 + 2)

g. 6 % (8 - 6 + 2) - (3 * 3) / 3

h. (12 % (5 / 2)) * 3 + (7 - 4)

i. (14 / 2) * 3 + 6 % 2

j. ((15 % 3) / 3) * (7 - 4) + 5

### Part 2
a. 5.5 * (3 + 1) - 2 / 2.0

b. 8 % 3 + (4.5 * 2) - 1 / 2.0

c. (7 / 2.0) * (4 + 3.5) - 6 % 2

d. (8 - 4) / 3 * 3.5 + 6 / 2.0

e. (9 - 3.5) * 2 * (7 - 5.5) + 4.0 / 8

f. 3.0 * (6 / 2) % 2 + (5 - 3.5)

g. (9 - 4) / 2.0 * (8 - 4) - 5 / 2

h. (5 / 2.0) * (7 - 4.5) + 6 % 2

i. (6.5 - 3) / 2 * (7 - 4) + 5 % 2

j. 3 * (5 / 2) % 2 + (7 - 3.0) / 2.0

## Problem0
Make a program that creates two variables: an int and a double.  Follow these instructions in the exact order below.
1. Create a variable of type `double` and store an int value into it.
2. Print out the value of the variable.
3. Run your program and observe the result.
4. Create a variable of type `int` and store a double value into it.
5. Print out the value of the variable.
6. Run myour program and observe the result.

Is it possible to store a double into an int?  Is it possible to store an int into a double?  Explain.

## Problem1
Write a program that takes a single integer and stores it in a variable. Your program should increase the value of this variable by one four times, printing "number is now " followed by its value each time, then decrease it by one four times, again printing "number is now " and the value each time. You must use unary operators to increase/decrease the value of the variable to receive full credit for this assignment.

Sample Run
```
Initial value: 24
number is now 25
number is now 26
number is now 27
number is now 28
number is now 27
number is now 26
number is now 25
number is now 24
```

## Problem2
Write a program which takes a positive three digit integer and prints out the digits one per line in order.

Hint: Integer division can give you one of the digits, a combination of Integer division and modulus can be used to get the second digit, and modulus alone will be used to get the other.

Sample run:
```
Three digit number: 678

Here are the digits:
8
7
6
```

## Problem3
Write a program which takes a four digit number then prints the digits of this number one per line in reverse order.

Hint: Break this challenge down into repetitions of the steps used for activity 1. Using multiple variables will let you store digits and intermediate results you need.

Sample run:
```
Four digit number:
5678

Here are the digits:
8
7
6
5
```

# Sample Solutions
## Problem0
```java
public class Problem0
{
  public static void main(String[] args)
  {
    double x = 4; // this works
    int y = 4.0; // this is an error
  }
}
```

## Problem1
```java
public class Problem1
{
  public static void main(String[] args)
  {
    int val = 24;
    System.out.println(val);
    val++;
    System.out.println("val is now: " + val);
    val--;
    System.out.println("val is now: " + val);
  }
}
```

## Problem2
```java
public class Problem2
{
  public static void main(String[] args)
  {
    int val = 867;
    System.out.println(val % 10);  // prints 7
    val /= 10;  // val is now 86
    System.out.println(val % 10);  // prints 6
    val /= 10;  // val is now 8
    System.out.println(val % 10);  // prints 8
  }
}
```
