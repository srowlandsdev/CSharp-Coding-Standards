# CSharp-Coding-Standards

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
