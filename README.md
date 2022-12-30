# C#
- [x] It is an object-oriented programming language created by Microsoft that runs on the .NET Framework.
- [x] C# is used to develop web apps, desktop apps, mobile apps, games and much more.
- [x] C# is pronounced "C-Sharp".

> C# is used for:
>* Mobile applications
>* Desktop applications
>* Web applications
>* Web services
>* Web sites
>* Games
>* VR
>* Database applications

# Syntax

```
using System;

namespace HelloWorld
{
  class Program
  {
    static void Main(string[] args)
    {
      Console.WriteLine("Hello World!");    
    }
  }
}
```

# Example explained

- Line 1: **using System** means that we can use classes from the System namespace.
- **Line 2:** A blank line. C# ignores white space.

- **Line 3:** namespace is used to organize your code, and it is a container for classes and other namespaces.

- **Line 4:** The curly braces {} marks the beginning and the end of a block of code.

- **Line 5:** class is a container for data and methods, which brings functionality to your program. Every line of code that runs in C# must be inside a class. In our example, we named the class Program.

- **Line 7:** Another thing that always appear in a C# program, is the Main method. Any code inside its curly brackets {} will be executed. You don't have to understand the keywords before and after Main. You will get to know them bit by bit while reading this tutorial.

- **Line 9:** Console is a class of the System namespace, which has a WriteLine() method that is used to output/print text. In our example it will output "Hello World!".

If you omit the using System line, you would have to write System.Console.WriteLine() to print/output text.

> **Note:** Every C# statement ends with a semicolon ;.

> **Note:** C# is case-sensitive: "MyClass" and "myclass" has different meaning.

# Keywords

C# contains reserved words that have special meaning for the compiler. These reserved words are called "keywords". Keywords cannot be used as an identifier.

# Access Modifier

> **Public** : The Public modifier allows any part of the program in the same assembly or another assembly to access the type and its members.

> Private : The Private modifier restricts other parts of the program from accessing the type and its members. Only code in the same class or struct can access it.

> Internal : The Internal modifier allows other program code in the same assembly to access the type or its members. This is default access modifiers if no modifier is specified.

> Protected : The Protected modifier allows codes in the same class or a class that derives from that class to access the type or its members.


# Data Types
It is a strongly-typed language. It means we must declare the type of a variable that indicates the kind of values it is going to store, such as integer, float, decimal, text, etc.
```
string stringVar = "Hello World!!";
int intVar = 100;
float floatVar = 10.2f;
char charVar = 'A';
bool boolVar = true;
```

# Variables
Variables are containers for storing data values.

> type variableName = value;

# Identifiers
All C# variables must be identified with unique names. These unique names are called identifiers.

> The general rules for naming variables are:
>* Names can contain letters, digits and the underscore character (_)
>* Names must begin with a letter
>* Names should start with a lowercase letter and it cannot contain whitespace
>* Names are case sensitive ("myVar" and "myvar" are different variables)
>* Reserved words (like C# keywords, such as int or double) cannot be used as names

# Type Casting
Type casting is when you assign a value of one data type to another type.

> In C#, there are two types of casting:

* Implicit Casting (automatically) - converting a smaller type to a larger type size ```char -> int -> long -> float -> double```

* Explicit Casting (manually) - converting a larger type to a smaller size type ```double -> float -> long -> int -> char```

> Type Conversion Methods
```
int myInt = 10;
double myDouble = 5.25;
bool myBool = true;

Console.WriteLine(Convert.ToString(myInt));    // convert int to string
Console.WriteLine(Convert.ToDouble(myInt));    // convert int to double
Console.WriteLine(Convert.ToInt32(myDouble));  // convert double to int
Console.WriteLine(Convert.ToString(myBool));   // convert bool to string
```
# Class
class is a template or blueprint that defines by user in which we define the properties & behaviour of objects.
```
class Student
{
    
}
```
A class can contain one or more constructors, fields, methods, properties, delegates, and events. They are called class members. A class and its members can have access modifiers such as public, private, protected, and internal, to restrict access from other parts of the program.

# Field
A class can have one or more fields. It is a class-level variable that holds a value. Generally, field members should have a private access modifier used with property.

# Object 
object is a instance of a class that represent the class and an object is an real entity that has state and behaviour.
```
Student myobj = new Student();
```

# Methods
A method is a block of code which only runs when it is called. You can pass data, known as parameters, into a method. Why use methods? To reuse code: define the code once, and use it many times.

A method can contain one or more statements to be executed as a single unit. A method may or may not return a value. A method can have one or more input parameters.
```
[access-modifier] return-type MethodName(type parameterName1, type parameterName2,...)
{
    

}
```
> Two Type of Methods
>* Static Method :- Using Class to call a Method
>* Non-Static Method or Instance Method :- Using Object to call a Method

> According to Parameters there are Two Type of Methods
>* Parameterized Methods
>* Non-Parameterized Methods

# Method Parameter
These keywords are applied to the parameters of a method.
- [x] ref
- [x] out
- [x] params


# Constructor
A constructor is a special type of method which will be called automatically when you create an instance of a class. A constructor is defined by using an access modifier and class name
```
<access-modifier> <class-name>(){ }
```