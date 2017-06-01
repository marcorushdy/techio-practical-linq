# LINQ Concepts: Method syntax
The other LINQ format is method syntax. The LINQ method syntax can do everything that query syntax can do, and more. It's just a different way to format the instructions.

### Method syntax example
Recall this example of query syntax:

```csharp
//// EMBED: LinqCourseEmbeddedCode/LinqConcepts1.cs, LINQ query syntax
```

This exact same instruction can be written in method syntax like this:

```csharp
//// EMBED: LinqCourseEmbeddedCode/LinqConcepts1.cs, LINQ method syntax
```

### Advantages of method syntax

I, personally, prefer method syntax over query syntax, and this is the format that will be used for the rest of this course. Here are some of the advantages of method syntax

 - All query syntax is automatically converted to method syntax at compilation time
 - Not all LINQ methods can be utilized with query syntax
 - Method syntax is stylistically more similar to other C# code

### Method syntax exercise

This is the exact same exercise as in the previous lesson. Now try to write it with method syntax.

The following code shows a LINQ query that returns the input `inValues` unmodified. Using the format of the above example, see if you can return only the strings that have `pattern` in them (using the `.Contains()` method of `string`) and order the list alphabetically.

@[Method Syntax Exercise]({"stubs": ["MethodSyntax1/MethodSyntax1.cs"], "command": "MethodSyntax1.UnitTest.Exercise1", "project": "exercises"})