[slide]
# If...else Statement
In an if-else statement, **`if`** condition evaluates to **`true`**, the then-statement runs. If condition is false, the else-statement runs

Because condition can't be simultaneously true and false, the then-statement and the else-statement of an if-else statement can never both run

In an if statement that doesn't include an else statement, if condition is true, the then-statement runs. If condition is false, control is transferred to the next statement after the if statement.

```csharp
if (condition)
{
  // then-statement
  // Commands to be executed if the condition is true
}
else
{
  // else-statement
  // Commands to be executed if the condition is false
}
```
[/slide]

[slide]
# Block of Code
The curly brackets ***\{\}*** introduce a **block** (a group of commands)

In case the ***if*** statement does **not** have curly brackets, only the code on the **next line** will be executed

```csharp
string color = "red";
if (color == "red") 
  Console.WriteLine("tomato");
else
  Console.WriteLine("banana");
Console.WriteLine("lemon"); /* <- Always executed */
```
```csharp
string color = "red";
if (color == "red")
{
  // Block of 2 commands
  Console.WriteLine("tomato");
  Console.WriteLine("strawberry"); 
}
else
{
  // Block of 2 commands
  Console.WriteLine("banana");
  Console.WriteLine("lemon");
}
```
[/slide]

[slide]
# Problem: Even or Odd
[code-task title="Even or Odd" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
Write a program, which checks if a number is **even** or **odd**

  * If it's even, print "**even**"
  * If it's odd, print "**odd**"
[/task-description]
[code-io /]
[/code-task]

# Sample Input and Output
|Input|Output|
|-----|------|
|4|even|
|7|odd|
|0|even|
[/slide]

[slide]
# Solution: Even or Odd
[code-task title="Even or Odd" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      int n = int.Parse(Console.ReadLine());
      if (n % 2 == 0) 
      {
        Console.WriteLine("even");
      }
      else 
      {
        Console.WriteLine("odd");
      }
    }
}
```
[/code-editor]
[task-description]
Write a program, which checks if a number is **even** or **odd**

  * If it's even, print "**even**"
  * If it's odd, print "**odd**"
[/task-description]
[code-io /]
[/code-task]

# Sample Input and Output
|Input|Output|
|-----|------|
|4|even|
|7|odd|
|0|even|
[/slide]

[slide]
# Problem: Greater Numbers
[code-task title="Greater Number" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
Write a program, which finds the greater of two numbers:

  * Read two **integers**
  * Find the greater number
  * Print ***"Greater number:"*** + the **greater** number
[/task-description]
[code-io /]
[/code-task]

# Sample Input and Output
|Input|Output|
|-----|------|
|4|Greater number: 8|
|8||
[/slide]

[slide]
# Solution: Greater Numbers
[code-task title="Greater Number" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      int num1 = int.Parse(Console.ReadLine());
      int num2 = int.Parse(Console.ReadLine());
      if (num1 > num2) 
      {
        Console.WriteLine("Greater number: " + num1);
      }
      else 
      {
        Console.WriteLine("Greater number: " + num2);
      }
    }
}
```
[/code-editor]
[task-description]
Write a program, which finds the greater of two numbers:

  * Read two **integers**
  * Find the greater number
  * Print ***"Greater number:"*** + the **greater** number
[/task-description]
[code-io /]
[/code-task]

# Sample Input and Output
|Input|Output|
|-----|------|
|4|Greater number: 8|
|8||
[/slide]
