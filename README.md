# .NET Core, C#, MVC, and Web APIs Oh My.

This week we're going to learn a bit more about c#, which is a language that lives in the .NET environment. When learning any new languages, it's important to do a lay of the land, survey the tools, and try to get some solid ground under your feet by trying to find familiar concepts in this strange new world. Please understand: **it is normal for this to feel foreign, strange, and like your legs are stuck in the mud!** Learning a new technology is never easy. The key is patience, taking good notes, and saving helpful references like tutorials and sample projects so you can continue learning from working examples.

C# is a great candidate to help us learn a new server-side language for a few reasons. First, the latest version of .NET, called .NET Core, is open-source, cross platform, and modern. This lets us write code that uses drastically different features from what we're used to: statically typed, compiled, and object-oriented (class based). We'll also get our first look at code-first database design, database migrations, high-level database functionality, and an "enterprise framework" approach to software development.

Throughout this exploration, you will be using Google to find answers to common questions, follow along with tutorials, read documentation, search error messages, and generally spend more time reading than writing.

When learning any new technology, there's a few questions to ask in the beginning. I encourage you to do some googling to get some context around the c# language or any other language that you're interested in learning. Some of these questions may not be answerable until you've started playing with the language a bit.

Spend some time (~30mins) googling some of these questions to see what you can uncover.

  - Is this language compiled or interpreted?
    - Most say C# is a compiled language because it compiles to bytecode (IL code) where IL is Intermediate Language.
    - bytecode is a computer object code that an interpreter converts into binary machine code so it can be read by a computer's      hardware processor.
  - Does this language use dynamic or static typing?
    - C# is considered statically typed and originally was only statically typed. After C# 4, dynamic elements were added to improve C#'s ability to exchange information with dynamically typed languages.
  - What editor do you use to write code in this language?
    - The most popular code editor for C# is Visual Studio Code. 
  - What plugins for the editor are popular?
    - C# for Visual Studio Code, offering intellisense, syntax highlighting, and debugging.
    - .NET Core Test Explorer, offering the dotnet test command which has a visual hierarchy of the test done in a tree layout.
  - Is this a stable language or something more experimental?
    - C# is a stable language having many experimental extensions.
  - When was the latest release of the language?
    - The most recent stable release was on November 8th 2021.
  - Who created this language?
    - Anders Hejlsberg designed the C# language.
  - What is the most popular framework that this language uses?
   - .NET Core is the most popular.
  - What is this language used for?
   - It can be used for web apps, games, and other software.
  - What platforms is this language meant to run on?
    - It can be run on Windows, Linux, and macOS using .NET Core.
  
Specifically about the language itself:
  - How do you get to 'Hello World'? 
    - Console.WriteLine("Hello World!");
  - How do you print to the console?
    - Console.WriteLine();
  - How do you run a program?
    - CTRL + F5 or CMD + F5
  - What kind of datatypes are there? 
    - int
    - long
    - float
    - double 
    - bool 
    - char 
    - string
  - How do you make a number, integer, decimal?
    - int number = 0;
    - int integer = 0;
    - float decimal = 1.1;
  - How do you make a string?
    - string myName = "David";
  - How do you make a collection / list / array?
    - Collection / List: var numbers = new List<int> {1, 2, 3, 4, 5};
    - Array: int[] arr1 = {1, 2, 3, 4, 5};
  - How do you write a function?
  
Once you have started working out these basic questions about the language itself, you can start to ask questions about the general ecosystem:

  - What package manager is used to install libraries?
    - NuGet
  - How do you write an HTTP API? Is there an http micro-framework or something built in?
  - How do you connect to a database?
  - How do you turn objects into JSON?
  - etc.
  
## Getting into C#

Once you have done some googling, its time to get to work. C# is unique in that there are some really great resources available from Microsoft, including an online tutorial. My recommendation is to do the following:

  1. Work through the [online tutorial](https://dotnet.microsoft.com/learn/dotnet/in-browser-tutorial/1). You don't need to install anything! It's just a friendly introduction to C#.
  2. Work through the [C# in 10 minutes](https://dotnet.microsoft.com/learn/dotnet/hello-world-tutorial/next) tutorial. This tutorial will also have you install the dotnet SDK, which is how you will write C# on your computer. ***Note: Install .NET 5 SDK, not .NET Core 3.1*** VS Code works great with C#, just be sure to also install the C# extension. ***Note:*** you will be using VS Code, not Visual Studio. Microsoft has done a good job at writing tutorials for both environments, but you should ignore any tutorial that specifically use Visual Studio.
  3. Continue learning about the language through the [online documentation](https://docs.microsoft.com/en-us/dotnet/csharp/tutorials/). The online portal is extensive and includes several tutorials including `Numbers in C#`, `Branches and Loops`, `List Collection`, and `Introduction to C#` (which includes some further exercises about classes).
  4. Read up on [Object Oriented Fundamentals in C#](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/object-oriented-programming) (at least the first 3/4)
  5. Read up on [how to build Web APIs with .NET Core](https://docs.microsoft.com/en-us/aspnet/core/tutorials/first-web-api?view=aspnetcore-3.1&tabs=visual-studio-code). The tutorial walks through building a "ToDo" app :). Many things may not make sense, that's OK. Get get a survey of the ideas.
  6. Google around for more introductions: "c# for beginners", "dotnet c# for javascript developers", etc.
  
### Additional Resources

The Microsoft online documentation has extensive introductory resources to c# and dotnet core in general. You can click through all of the resources on the left navigation pane to learn more. For example, the [Tour of C#](https://docs.microsoft.com/en-us/dotnet/csharp/tour-of-csharp/) article is a helpful read that covers program structure, types and variables, expressions, statements, etc. The introduction to classes is useful but it's OK if you don't quite get to it.

## dotnet trivia questions (Group Activity)

Before continuing, please make sure that you have completed the following:

  - You have installed the dotnet SDK and can run `dotnet --version` from the command line successfully
  - You can use VS Code to build a dotnet application (using `dotnet run` or `dotnet watch run`) and are using the c# extension
  - You have built and executed your first 'hello world' c# console application successfully.
  - You have finished at least a couple of the introductory c# tutorials

The following questions are meant to help you build a foundation of vocabulary, to be completed after you've finished the introductory tutorials. Every new environment comes with new paradigms, keywords, and ideas. Some of these things are directly applicable to things you've already learned in other environments, others may be new. Some may be simply technical (like syntax), others may be completely new to you (like inventions specific to the .NET environment).

Work through these trivia problems as a group. Discuss and see what you can uncover!

  - What similarities stick out to you between C# and JavaScript? What major differences?
  - What does `var` in c# do compared to JavaScript?
  - What is the difference between .NET Core and .NET Framework?
  - What languages can you use in .NET Core?
  - What does it mean to say that c# is a statically typed language?
  - How do you create a new dotnet project from the command line?
  - What is NuGet? How do you use it within dotnet?
  - How do you represent a string in c#? What about numbers / integers / decimals?
  - How do you create a List of integers? What about a list of strings?
  - How do you loop over a list? How do you do an old-school for loop?
  - What is `using` used for?
  - How do you write a function that takes in a string as an argument and console logs the string?
  - How do you write a function that takes no arguments but returns an instance of a class `Human`?
  - What is does a `public void` function do?
  - What is a class?
  - What is a class property vs class method?
  - What is the difference between an abstract and virtual class method?
  - What does it mean for a class property to be `private` vs `public`? What about `protected`?
  - What are getters and setters?

More advanced topics, specific for web app development:
  - What is 'Code First' database design?
  - What are database migrations?
  - What does MVC standfor? How is each part used in a modern web app with react?
  - What is a dbContext as it relates to .NET?
