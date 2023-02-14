# C# Asp.Net
Free. Cross-platform. Open source. A developer platform for building all your apps. Official handle of the .NET team at Microsoft.

### Index

1. [ Introduction. ](#introduction)
2. [ Web Pages Razor. ](#razor)
   - [ Razor Markup. ](#razor)
   - [ Razor Syntax for C#. ](#razorsyntax)

<a name="introduction"></a>
- ## Introduction

### .Net
.NET is a free, cross-platform, open source developer platform for building many different types of applications.
With .NET, you can use multiple languages, editors, and libraries to build for web, mobile, desktop, games, IoT, and more.

### Languages
You can write .NET apps in C#, F#, or Visual Basic.

C# is a simple, modern, object-oriented, and type-safe programming language.
F# is a programming language that makes it easy to write succinct, robust, and performant code.
Visual Basic is an approachable language with a simple syntax for building type-safe, object-oriented apps.

### Cross Platform
Whether you're working in C#, F#, or Visual Basic, your code will run natively on any compatible operating system. You can build many types of apps with .NET. Some are cross-platform, and some target a specific set of operating systems and devices.

### One consistent API
.NET provides a standard set of base class libraries and APIs that are common to all .NET applications.

Each app model can also expose additional APIs that are specific to the operating systems it runs on, or the capabilities it provides. For example, ASP.NET is the cross-platform web framework that provides additional APIs for building web apps that run on Linux or Windows.

<a name="razor"></a>
- ## ASP.NET Web Pages - Adding Razor Code

### Razor Markup

ASP.NET Web Pages use Razor markup with C# or VB code.

Razor is a simple markup syntax for embedding server code (C# or VB) into ASP.NET web pages.

Example:
````
<!DOCTYPE html>

<html lang="en">
<head>
     <meta charset="utf-8" />
     <title>Web Pages Demo</title>
</head>
<body>
     <h1>Hello Web Pages</h1>
     <p>The time is @DateTime.Now</p>
</body>
</html>
````

<a name="razorsyntax"></a>
### Razor Syntax for C#

- C# code blocks are enclosed in @{ ... }
- Inline expressions (variables or functions) start with @
- Code statements end with semicolon
- Variables are declared with the var keyword, or the datatype (int, string, etc.)
- Strings are enclosed with quotation marks
- C# code is case sensitive
- C# files have the extension .cshtml

Example:
````
<!-- Single statement block -->
@{ var myMessage = "Hello World"; }

<!-- Inline expression or variable -->
<p>The value of myMessage is: @myMessage</p>

<!-- Multi-statement block -->
@{
var greeting = "Welcome to our site!";
var weekDay = DateTime.Now.DayOfWeek;
var greetingMessage = greeting + " Today is: " + weekDay;
}
<p>The greeting is: @greetingMessage</p>
````

<a name=""></a>
### Page Layout

