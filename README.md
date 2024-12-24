# Use-Generative-Ai-for-software-developmentware-
its my first way to learn ai by my own using IBM Open e - learning Ecosystem
Estimated duration
 1 hour
Version information
Version: 1.0
Date: 19-August-2024
Release notes: Generally available (GA) version of the module released.

// Learning objectives



>Identify the benefits of using generative AI for software development



>Describe how generative AI is used to write code



>Identify common issues with AI-generated code



>Use IBM watsonx in a simulation to generate code

// we all know making website is not easy if u don't know how to code but we can use generative ai to make codes by just asking them 



> like we want a code for python or java we can just ask them .



//How does generative AI make learning to code easier for beginners?



>It provides instant help and feedback, reducing the learning curve.



>It writes code for you, allowing you to save time.

// its easy to make lines of codes with simple prompts



>You are new to coding and feel overwhelmed by the complexity of learning to program.



>as we all know prompt is the future to write codes easy for us because it makes code to o and 1 with complier but here we can make prompt to 0 and 1 with generative ai .



>0s and 1s (machine code )




>There are amazing generative AI tools like IBM watsonx, ChatGPT, Claude, Google’s Bard, and Microsoft’s Copilot are changing how you approach coding. 

//What is a prompt? 
>A prompt is like giving the AI a set of clear instructions on what you want it to create. It’s like saying, “Here’s my idea. Can you make something like this?”

//how to use a prompt to get AI to generate a code.
>1. Create a prompt-You provide a clear prompt.
You start by describing what you want the code to do. This could be a function, a program, or a specific feature.



Example prompt: “Create a function in Python that calculates the square of a number.”

>2. AI interprects the result-The AI interprets the request-
The AI understands the context of your request, recognizing what kind of code is required to meet your needs. It leverages its training on a vast amount of code data to match patterns and structures that fit the description in your prompt.

>3. AI generates the code- The AI generates the code.
Based on the interpretation of the prompt, the AI generates code that accomplishes the task you described. It ensures the code follows the syntax and conventions of the specified programming language.

//Let’s review a few examples of writing new code with simple prompts.
>prompt-Write a Python program to add two numbers and print the sum.
>AI generates -
number1 = 5

number2 = 3

 

sum = number1 + number2

 

print("The sum of", number1, "and", number2, "is", sum)
>prompt-Write a JavaScript program to check if the number is even and print “The number is even.” when it’s even and “The number is odd.” when it’s odd.
>AI generates -



let number = 7;

 

if (number % 2 === 0) {

     console.log("The number is even.");

} else {

     console.log("The number is odd.");

}

>prompt-Write a C++ program to find the greater of the two numbers and print it.
>AI generates -



#include <iostream>

using namespace std;

 

int main() {

     int number1 = 8;

     int number2 = 12;

 

     if (number1 > number2) {

         cout << "The greater number is " << number1 << endl;

    } else {

         cout << "The greater number is " << number2 << endl;

    }

 

     return 0;

}

>prompt-Write an HTML code to take a name as input and display greet them by their name on the click of a button.
>AI generates -



<!DOCTYPE html>

<html>

<head>

     <title>Greeting App</title>

     <script>

         function greetUser() {

             // Get the input value (name)

             var name = document.getElementById("nameInput").value;

 

             // Display the greeting message

             document.getElementById("greetingMessage").innerHTML = "Hello, " + name + "!";

         }

     </script>

</head>

<body>

     <h1>Greeting App</h1>

     <label for="nameInput">Enter your name:</label>

     <input type="text" id="nameInput" placeholder="Your name here">

     <button onclick="greetUser()">Greet Me</button>

     <p id="greetingMessage"></p>

</body>

</html>

// Convert existing code to a different programming language.
>Generative AI can also help you convert code from one programming language to another. This is useful if you’re familiar with one language but need your code in another.

//Why would you convert code from one programming language to another?
>a. Language Flexibility -



Generative AI allows you not to restrict yourself to any programming language. You can work with the language you’re most comfortable with and let the AI handle the translation.
>b. Platform compatibility



Different platforms (such as Android and iOS) may support different programming languages. Converting code allows the software to run on a new platform that requires a different language.
>. Integration with other systems



Sometimes, a project may need to integrate with other systems or software that are built using a different programming language. Converting code ensures compatibility between systems.
>. Legacy system updates



Older systems might be written in outdated or less efficient languages. Converting these systems to modern languages can improve maintainability, performance, and security.


//Let’s review a few examples of converting code from one programming language to another using simple prompts.


>a.Prompt- Convert a Python function that adds two numbers to JavaScript.
def add_numbers(a, b):

    return a + b

> AI generates-


def multiply(a, b):

    return a * b


function addNumbers(a, b) {

     return a + b;

}

>b.prompt - Convert a COBOL program that prints “Hello, World!” to Python.

 

IDENTIFICATION DIVISION.

PROGRAM-ID. HelloWorld.

PROCEDURE DIVISION.

    DISPLAY 'Hello, World!'.

    STOP RUN.


>AI generates -


print("Hello, World!")



//Common issues found in AI-generated code.



> One of the biggest concerns is the potential for generating incorrect or poor-quality code. AI models draw from existing data, and if that data contains errors or poor coding practices, the AI might replicate these issues. Additionally, AI-generated code may not understand the context and requirements that a human developer possesses, leading to code with errors, or even worse, hallucinations.



//Select each tab to learn more about errors in AI-generated code.


>accuracy and errors - 

Sometimes, the code does not work as you expect or has errors. The AI can generate code that seems correct but doesn’t perform the task properly.



Example: If you ask the AI to write a function to calculate the average of a list of numbers, the code might work in most cases but could fail if it doesn’t handle special situations, like an empty list. If the code doesn’t check for an empty list, it might give an error or an incorrect result, such as dividing by zero. This can cause unexpected issues and bugs that must be fixed to ensure the code works correctly.


>context misunderstanding -


The AI might not fully understand your request’s details or overall context, which can lead to code that doesn’t meet your needs.



Example: If you ask the AI to generate code for processing customer feedback but don’t specify that you need to handle both text and numerical ratings, the AI might create code that only processes text comments. This means the numerical ratings would be missed, leading to incomplete data processing and missing important insights.

>code Quality -


The AI-generated code might work but might not be well-organized or easy to understand. This can make it harder to maintain or update the code later.



Example: The code might function correctly but may not be written clearly or use consistent naming conventions. This can be confusing for someone who needs to work with it later. For instance, the code might use vague variable names or lack comments explaining what each part does, making it harder to understand or modify in the future.


> security status -


The AI-generated code might have security flaws if it doesn’t follow best practices for protecting data and preventing unauthorized access.



Example: If you ask the AI to create a login system for a website, the generated code might let users log in but might not use encryption to protect passwords. It might also fail to check if input data is safe, allowing malicious users to exploit these weaknesses and gain unauthorized access to sensitive information.



// Basic troubleshooting techniques 


>Look at the code for any obvious mistakes, like missing semicolons or typos.


Run the code in a development environment that highlights syntax errors. Many Integrated Development Environments (IDEs) have built-in tools to help with this.

>run the code with different inputs to see if it behaves as expected.


Create test cases that cover a range of scenarios, including edge cases like very large numbers and empty inputs.

>Read any comments in the code or external documentation to understand what it’s supposed to do.



Look for comments within the code or external documentation that explains the code’s purpose and usage.

>If the code is too complex, break it down into smaller parts and test each part individually.



Isolate sections of the code and test them separately to identify where things might be going wrong.

>If you’re stuck, ask for help from online communities or forums.


Post a clear description of the problem, including the code and what you’re trying to achieve, to get advice from experienced programmers.


//Points to remember
>Key concepts

1
Generative AI is a type of artificial intelligence that can generate new content.

2
Benefits of using generative AI for software development:

Can take a few instructions from you and turn them into a complete program
Can suggest how to complete certain sections of code or even write new parts for you
Can find and fix errors in the code
Can save time by handling tedious coding tasks
Makes learning to code much easier
3
A prompt is like giving AI a set of clear instructions on what you want it to create.

4
Process of writing code using generative AI:

You provide a clear prompt.
The AI interprets the request.
The AI generates the code.
5
Reasons for converting code from one programming language to another:

Provides you the flexibility to work with the language of your choice
Allows the software to run on a new platform that requires a different language
Enables integration with other systems or software that are built using a different programming language
Improves maintainability, performance, and security of legacy systems
6
Common issues found in AI-generated code:

The AI can generate code that seems correct but doesn’t perform the task properly.
The AI might not fully understand your request’s details or overall context.
The AI-generated code might work but might not be well-organized or easy to understand.
The AI-generated code might have security flaws.


//Learning objectives

>Now that you’ve completed this module, you should be able to:

•
Identify the benefits of using generative AI for software development

•
Describe how generative AI is used to write code

•
Identify common issues with AI-generated code

•
Use IBM watsonx in a simulation to generate code
