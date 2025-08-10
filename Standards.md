> This document is based on multiple public sources on GitHub repositories, articles, website and microsoft [internal coding guidlines][ms-coding-guidelines].
# CSharp-Coding-Standards
## Why Should I Use This?
We've all looked at code at one point or another and gone "That could have been better if person X did this" or "Why does the class not have a summary". In short this standard serves as a lesson from others on what not to do when using C# and how you can avoid mistakes, pitfalls and get a clean, and in some cases more optimised start to your codebase. It is considerate for you and whoever will likely have to view and maintain your code down the road if you are part of a team.

## Sources
https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/coding-conventions
https://www.geeksforgeeks.org/c-sharp/c-sharp-coding-standards/
https://www.dofactory.com/csharp-coding-standards#
https://google.github.io/styleguide/csharp-style.html
https://medium.com/@shubhadeepchat/c-coding-standards-f72df288f57c
https://github.com/hassanhabib/CSharpCodingStandard/blob/master/4.%20Methods.md
https://gist.github.com/colin-gourlay/c419390066b22c4b2d4f


## Classes
Utilise the PascalCase convention to make a distinction from variables

## Methods
Utilise the PascalCase convention to make a distinction from variables

## Variables
### General
- Camel Case

Always declare the properties as private so as to achieve Encapsulation and ensure data hiding.

```csharp
// Correct
private int objectCount { get; set; }

// Avoid
public int objectCount { get; set; }
```

### String
- Use string interpolation to concatenate short strings:
```csharp
string displayName = $"{nameList[n].LastName}, {nameList[n].FirstName}";
```

## Enums

## Namespaces

## Interfaces
Prefix with I

## Files

## Constants
- When declaring constant variables always stick to using the UPPERCASE / SCREAMING convention as shown below:
```csharp
// Correct
public const int MIN = 18;
public const int MAX = 60;

// Avoid
public const int Min = 18;
public const int Max = 60;
```


- In addition when declaring variables with multiple words/elenments defer to SCREAMING_SNAKE convention as shown below:
```csharp
// Correct
public const int MIN_VAL = 18;
public const int MAX_VAL = 60;

// Avoid
public const int Min_Val = 18;
public const int Max_Val = 60;
```

## Structs

## Constructors

## Exception Handling

## For Loops

## Comments
- Use single-line comments (//) for brief explanations within the code.
- Avoid excessive comments; aim for self-explanatory code.
- Include a summary, remarks, and example sections in your XML comments.
- Avoid multi-line comments for longer explanations.
- Place the comment on a separate line, not at the end of a line of code.
- Begin comment text with an uppercase letter.
- End comment text with a period.
- Insert one space between the comment delimiter and the comment text.

For classes, methods and properties use XML comments as a standard like this:
```csharp
    /// <summary>
    /// Template Class.
    /// </summary>
    public class MyClass
    {
        // Class implementation
    }
```

### Copyrights

Sourced from hassanhabib/CSharpCodingStandard

##### Do
```csharp
    // ---------------------------------------------------------------
    // Copyright (c) Coalition of the Good-Hearted Engineers
    // FREE TO USE TO CONNECT THE WORLD
    // ---------------------------------------------------------------
```

##### Don't
```csharp

    //----------------------------------------------------------------
    // <copyright file="StudentService.cs" company="OpenSource">
    //      Copyright (C) Coalition of the Good-Hearted Engineers
    // </copyright>
    //----------------------------------------------------------------

```

##### Also, Don't
```csharp
   /* 
    * ==============================================================
    * Copyright (c) Coalition of the Good-Hearted Engineers
    * FREE TO USE TO CONNECT THE WORLD
    * ==============================================================
    */
```
