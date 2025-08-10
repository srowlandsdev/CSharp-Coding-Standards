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
Use string interpolation to concatenate short strings

## Enums

## Namespaces

## Interfaces
Prefix with I

## Files

## Constants
Uppercase

## Structs

## Constructors

## Exception Handling

## Comments
- Use single-line comments (//) for brief explanations within the code.
- Avoid excessive comments; aim for self-explanatory code.
- Include a summary, remarks, and example sections in your XML comments.

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
