# Introduction to Javascript


JavaScript is primarily known as the language of most modern web browsers.

JavaScript is a powerful, flexible, and fast programming language now being used for increasingly complex web development and beyond!

Since JavaScript remains at the core of web development, it’s often the first language learned by self-taught coders eager to learn and build. 

We’re excited for what you’ll be able to create with the JavaScript foundation you gain here. JavaScript powers the dynamic behavior on most websites, including this one.


# Console

The console is a panel that displays important messages, like errors, for developers. 

Much of the work the computer does with our code is invisible to us by default. If we want to see things appear on our screen, we can print, or log, to our console directly.

In JavaScript, the console keyword refers to an object, a collection of data and actions, that we can use in our code. Keywords are words that are built into the JavaScript language, so the computer recognizes them and treats them specially.

One action, or method, that is built into the console object is the .log() method. When we write console.log() what we put inside the parentheses will get printed, or logged, to the console.

```
console.log(5); 
```

##  Class work

Use the console.log code in the editor to log your age to the console.

Run your code when you are ready to see the result.

## Video Explanation on Console.log() - https://youtu.be/lMAwyR5IZi8
Must watch this video.



# Comments

Programming is often highly collaborative. 

In addition, our own code can quickly become difficult to understand when we return to it— sometimes only an hour later! 

For these reasons, it’s often useful to leave notes in our code for other developers or ourselves.

There are two types of code comments in JavaScript:

1 A single line comment will comment out a single line and is denoted with two forward slashes // preceding it.

```
// Prints 5 to the console
console.log(5);
```

You can also use a single line comment to comment after a line of code:

```
console.log(5);  // Prints 5 
```

2 A multi-line comment will comment out multiple lines and is denoted with /* to begin the comment, and */ to end the comment.

```
/*
This is all commented 
console.log(10);
None of this is going to run!
console.log(99);
*/
```

You can also use this syntax to comment something out in the middle of a line of code:

```
console.log(/*IGNORED!*/ 5);  // Still just prints 5 
```

# Data Types

Data types are the classifications we give to the different kinds of data that we use in programming. 

In JavaScript, there are seven fundamental data types:


- Number: Any number, including numbers with decimals: 4, 8, 1516, 23.42.
- String: Any grouping of characters on your keyboard (letters, numbers, spaces, symbols, etc.) surrounded by single quotes: ' ... ' or double quotes " ... ", though we prefer single quotes. Some people like to think of string as a fancy word for text.
- Boolean: This data type only has two possible values— either true or false (without quotes). It’s helpful to think of booleans as on and off switches or as the answers to a “yes” or “no” question.
- Null: This data type represents the intentional absence of a value, and is represented by the keyword null (without quotes).
- Undefined: This data type is denoted by the keyword undefined (without quotes). It also represents the absence of a value though it has a different use than null. undefined means that a given value does not exist.
- Symbol: A newer feature to the language, symbols are unique identifiers, useful in more complex coding. No need to worry about these for now.
- Object: Collections of related data.


The first 6 of those types are considered primitive data types. They are the most basic data types in the language. Objects are more complex, and you’ll learn much more about them as you progress through JavaScript.



# Arithmetic Operators

Basic arithmetic often comes in handy when programming.

An operator is a character that performs a task in our code. JavaScript has several built-in arithmetic operators, that allow us to perform mathematical calculations on numbers. These include the following operators and their corresponding symbols:

- Add: ```+```
- Subtract: ```-```
- Multiply: ```*```
- Divide: ```/```
- Remainder: ```%```


The first four work how you might guess:

```
console.log(3 + 4); // Prints 7
console.log(5 - 1); // Prints 4
console.log(4 * 2); // Prints 8
console.log(9 / 3); // Prints 3
```


# String Concatenation

Operators aren’t just for numbers! When a + operator is used on two strings, it appends the right string to the left string:

```
console.log('hi' + 'ya'); // Prints 'hiya'
console.log('wo' + 'ah'); // Prints 'woah'
console.log('I love to ' + 'code.')
// Prints 'I love to code.'
```

This process of appending one string to another is called concatenation. 

Notice in the third example we had to make sure to include a space at the end of the first string. 

The computer will join the strings exactly, so we needed to make sure to include the space we wanted between the two strings.

```
console.log('front ' + 'space'); 
// Prints 'front space'
console.log('back' + ' space'); 
// Prints 'back space'
console.log('no' + 'space'); 
// Prints 'nospace'
console.log('middle' + ' ' + 'space'); 
// Prints 'middle space'
```

Just like with regular math, we can combine, or chain, our operations to get a final result:

```
console.log('One' + ', ' + 'two' + ', ' + 'three!'); 
// Prints 'One, two, three!'
```

# Properties

 All data types have access to specific properties that are passed down to each instance. 
 
 For example, every string instance has a property called length that stores the number of characters in that string. 
 
 You can retrieve property information by appending the string with a period and the property name:

```
console.log('Hello'.length); // Prints 5
```

The ```.``` is another operator! We call it the dot operator.

In the example above, the value saved to the length property is retrieved from the instance of the string, 'Hello'. The program prints 5 to the console, because Hello has five characters in it.


# Methods

Remember that methods are actions we can perform. Data types have access to specific methods that allow us to handle instances of that data type. 

JavaScript provides a number of string methods.

We call, or use, these methods by appending an instance with:

- a period (the dot operator)
- the name of the method
- opening and closing parentheses

E.g. ```'example string'.methodName().```

```
console.log('hello'.toUpperCase()); // Prints 'HELLO'
console.log('Hey'.startsWith('H')); // Prints true
```

# Built-in Objects

In addition to console, there are other objects built into JavaScript. Down the line, you’ll build your own objects, but for now these “built-in” objects are full of useful functionality.

For example, if you wanted to perform more complex mathematical operations than arithmetic, JavaScript has the built-in Math object.

The great thing about objects is that they have methods! Let’s call the .random() method from the built-in Math object:

```
console.log(Math.random()); // Prints a random number between 0 and 1
```

The example above will likely evaluate to a decimal. To ensure the answer is a whole number, we can take advantage of another useful Math method called Math.floor().

```
Math.floor(Math.random() * 50);
```

Math.floor() takes a decimal number, and rounds down to the nearest whole number.

```
console.log(Math.floor(Math.random() * 50)); // Prints a random whole number between 0 and 50
```

