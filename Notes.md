
# ► Pluralsight - C# Fundamentals

    .NET 
        > CLR (Common Language Runtime) - BCL (Base Class Library) 

&nbsp;

## Requiriments

.NET SDK
Text Editor

&nbsp;

## Creating the Project using .NET CLI

• Folder structure

    mkdir gradebook
    cd gradebook
    mkdir src
    mkdir test
    cd src
    mkdir GradeBook

• Creating the Project

    dotnet new console netcoreapp2

&nbsp;

## Run Project

• Run using CLI

Execute `dotnet run` inside folder of project

Or

Execute `dotnet run --project src\GradeBook` if it is outside the project folder

Or 

For run directly the assembly execute `dotnet bin\Debug\netcoreapp2.2\GradeBook.dll `


• Run using VS Code

Ctrl + F5

&nbsp;

## Architecture

• dotnet build 

Translates or transforms the source code into binary codes to be interpreted by the computer, the code is transformed into a dll file, an assembly that is the output of the compiler.
This file is located in the bin (binary) > debug > netcoreapp2.2 (.NET Version)

&nbsp;

## Strings

• Concatenation

    "Hello " + args[0] + "!"

• Interpolation

    $"Hello {args[0]} !"

&nbsp;

## Parsing parameters to the Main method (args)

• On CLI

    dotnet run -- Teste

    dotnet run -- MyName

• On VS Code

Add the parameter on .vscode folder > `launch.json`:

    "args": [
        "MyName"
    ]

&nbsp;

## Array

    var numbers = new double[] { 12.7, 10.3, 6.11 };

The compiler will discover the data type of the array, we can use implicit type:

    var numbers = new [] { 12.7, 10.3, 6.11 };

## List

To use the array, we need to know how many items we will have or initialize the array with some values. To solve this, we use a List, which is dynamic.

    List<double> grades = new List<double>();

The compiler will discover the data type of the List, we can use implicit type:

    var grades = new List<double>();

## Decimal Formatting

One decimal place:

    Console.WriteLine($"The average grade is {result:N1}");

Two decimal place: 

    Console.WriteLine($"The average grade is {result:N2}");




  
