# CSharp-Coding-Standards

## Classes
Pascal Case

## Methods
Pascal Case

## Variables
### General
Camel Case
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
