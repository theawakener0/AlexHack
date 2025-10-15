# Intro into Programming with C++

## Introduction

Hi, in this bootcamp, we will learn something different than you think, something new and interesting. We will learn not only how to code but also how to think like a programmer. We will the foudational aspects of programming and problem solving. We will learn how to break down a problem into smaller parts and how to solve each part step by step. We will also learn how to write clean and efficient code that is easy to read and understand.

The key is not to memorize the syntax of a programming language but to understand the logic behind it. Once you understand the logic, you can easily learn any programming language.

And The best thing is that we will use C++ as our programming language. C++ is a powerful language that is widely used in various fields such as game development, system programming, and embedded systems. It is also a great language for beginners because it teaches you the fundamentals of programming and helps you develop a good problem solving skills.

And also we choose it because it is one of the best languages to learn programming concepts that can be applied to other languages as well. (We love it)...

So, Let's get started! to the world of programming.

But before we start coding, let's first understand what programming is and what a programming language is.

### What is Programming?

Programming is the process of creating a set of instructions that tell a computer how to perform a specific task. It is a way of communicating with the computer to make it do what we want it to do. Programming involves writing code in a programming language, which is a set of rules and syntax that the computer can understand.

### What is a Programming Language?

A programming language is a formal language that consists of a set of instructions that can be used to create software programs. It is a way of expressing algorithms and data structures in a way that a computer can understand and execute. There are many programming languages available, each with its own syntax and rules. Some popular programming languages include C++, Python, Java, and JavaScript.

### How to Write Code?

Writing code involves using a programming language to create a set of instructions that the computer can understand and execute. Here are the basic steps to write code:
1. Choose a programming language: Select a programming language that is suitable for the task you want to accomplish.
2. Set up a development environment: Install the necessary software and tools to write and run code in your chosen programming language.
3. Write the code: Use a text editor or an integrated development environment (IDE) to write the code using the syntax and rules of the chosen programming language.
4. Test the code: Run the code to see if it works as expected and fix aerrors or bugs that may arise.
5. Debug the code: Use debugging tools to identify and fix any errors or issues in the code.
6. Refactor the code: Improve the code by making it more efficient, readable, and maintainable.
7. Document the code: Add comments and documentation to explain the purpose and functionality of the code.
8. Share the code: Share the code with others by publishing it on a code repository or sharing it with colleagues.
9. Maintain the code: Update and maintain the code as needed to ensure it continues to work as expected and meets the requirements of the task.

### The Philosophy of programming

"Code is not just instructions for machines, it's the crystallization of human thought. Every function, every variable name, every architectural decision reflects the mind of its creator and a path for the human evolution."


## C++

### How to install C++?

If you are using Windows, you can download Code::Blocks from [here](http://www.codeblocks.org/downloads/26). Make sure to download the version that includes MinGW, which is a compiler for C++ or Download Visual Studio from [here](https://code.visualstudio.com/). Make sure to select the "Desktop development with C++" workload during installation and install MinGW from [here](https://code.visualstudio.com/docs/languages/cpp).

If you are using macOS, you can install Xcode from the App Store. Xcode includes a C++ compiler and an integrated development environment (IDE) for writing and running C++ code.

If you are using Linux, you can install the GNU Compiler Collection (GCC) by running the following command in the terminal:
```bash 
sudo apt install build-essential
```
or use your package manager to install GCC.


### Your first C++ program

Now that you have installed a C++ compiler, let's write your first C++ program. Open your text editor or IDE and create a new file named `hello.cpp`. Type the following code into the file:

```cpp
#include <iostream>

using namespace std;

int main() {
    cout << "Hello, World!" << endl;
    return 0;
}
```

This code includes the `iostream` library, which allows us to use input and output streams. The `using namespace std;` line allows us to use standard library functions without having to prefix them with `std::`. The `main()` function is the entry point of the program, where the execution starts. The `cout` statement prints "Hello, World!" to the console, and `endl` adds a new line after the output. Finally, the `return 0;` statement indicates that the program has completed successfully.

To compile and run the program, open a terminal or command prompt, navigate to the directory where you saved the `hello.cpp` file, and run the following commands:

```bash
g++ hello.cpp -o Hello
```

```bash
./Hello # on Windows use Hello.exe
```

### Variables and Data Types

In C++, a variable is a named storage location that holds a value of a specific data type. A data type defines the type of data that can be stored in a variable, such as integers, floating point numbers, characters, and strings.

Here are some common data types in C++:

| Data Type | Description                          | Example          |
|-----------|--------------------------------------|------------------|
| int       | Integer (whole number)               | int age = 25;    |
| float     | Floating point number (decimal)      | float pi = 3.14; |
| double    | Double precision floating point      | double e = 2.71; |
| char      | Single character                     | char grade = 'A';|
| string    | Sequence of characters (text)        | string name = "John"; |
| bool      | Boolean value (true or false)        | bool isStudent = true; |
| long      | Long integer (larger range than int) | long population = 7800000000; |

To declare a variable in C++, you need to specify the data type followed by the variable name. You can also initialize the variable with a value at the time of declaration. Here are some examples:

```cpp
int age = 25;
float pi = 3.14;
char grade = 'A';
string name = "John";
bool isStudent = true;
long population = 7800000000;
```
You can also declare multiple variables of the same data type in a single line:

```cpp
int x = 10, y = 20, z = 30;

int a, b, c; // declaration without initialization

a = 5; // initialization later
b = 15;
c = 25;
```

You can use variables in your code to store and manipulate data. For example, you can perform arithmetic operations on integer and floating point variables:

```cpp
int x = 10;
int y = 20;

int sum = x + y; // sum is 30

float pi = 3.14;
float radius = 5.0;

float area = pi * radius * radius; // area is 78. 
```
So lets try to use variables in our `hello.cpp` program. Modify the code as follows:

```cpp
#include <iostream>

using namespace std;

int main() {
    string name;
    cout << "Enter your name: ";
    cin >> name; // take input from user
    cout << "Hello, " << name << "!" << endl; // use variable in output
    return 0;
}
```

In this modified code, we declare a variable `name` of type `string` to store the user's name. We use the `cin` statement to take input from the user and store it in the `name` variable. Finally, we use the `name` variable in the output statement to greet the user by their name.

### comments

Comments are used to add notes or explanations to your code. They are ignored by the compiler and do not affect the execution of the program. Comments are useful for documenting your code and making it easier to understand for yourself and others.

In C++, there are two types of comments:

1. Single-line comments: These comments start with `//` and continue until the end of the line. They are used for brief explanations or notes.

```cpp
// This is a single-line comment

int x = 10; // This is also a single-line comment
```

2. Multi-line comments: These comments start with `/*` and end with `*/`. They can span multiple lines and are used for longer explanations or notes.

```cpp
/* This is a multi-line comment
   It can span multiple lines
   and is useful for longer explanations */

int y = 20; /* This is also a multi-line comment */
```
You can use comments in your code to explain the purpose of variables, functions, and other parts of your code. For example, you can add comments to the `hello.cpp` program as follows:

```cpp
#include <iostream>

using namespace std;

// This is the main function where the program execution starts
int main() {
    string name; // Declare a variable to store the user's name
    cout << "Enter your name: "; // Prompt the user to enter their name
    cin >> name; // Take input from the user and store it in the 'name' variable
    cout << "Hello, " << name << "!" << endl; // Greet the user by their name
    return 0; // Indicate that the program has completed successfully
}
```
In this code, we have added comments to explain the purpose of the `main()` function, the `name` variable, and the input and output statements. This makes the code easier to understand for anyone who reads it.

### Basic Input and output

In C++, input and output are handled using the `iostream` library, which provides the `cin` and `cout` objects for reading input from the user and writing output to the console, respectively.

To use `cin` and `cout`, you need to include the `iostream` library at the beginning of your program:

```cpp
#include <iostream>

using namespace std;

int main() {
    // Your code here
    return 0;
}
```

The `cout` object is used to write output to the console. You can use the insertion operator (`<<`) to send data to `cout`. For example:

```cpp
cout << "Hello, World!" << endl; // Output a strings
````

The `cin` object is used to read input from the user. You can use the extraction operator (`>>`) to get data from `cin`. For example:

```cpp
string name;

cout << "Enter your name: "; // Prompt the user to enter their names
cin >> name; // Read the input and store it in the 'name' variables
cout << "Hello, " << name << "!" << endl; // Greet the user by their name
```

Let's leave thr input and output topic now and return to it later when we learn more about C++.

### Basic Operators

Operators are special symbols or keywords that perform specific operations on one or more operands (variables or values). In C++, there are several types of operators, including arithmetic, relational, logical, assignment, and bitwise operators.

Here are some common operators in C++:

| Operator | Description                          | Example          |
|----------|--------------------------------------|------------------|
| +        | Addition                             | int sum = a + b; |
| -        | Subtraction                          | int diff = a - b;|
| *        | Multiplication                       | int prod = a * b;|
| /        | Division                             | int quot = a / b;|
| %        | Modulus (remainder)                  | int rem = a % b; |
| ++       | Increment (increase by 1)            | a++;             |
| --       | Decrement (decrease by 1)            | b--;             |
| ==       | Equal to                             | if (a == b) {}   |
| !=       | Not equal to                         | if (a != b) {}   |
| >        | Greater than                         | if (a > b) {}    |
| <        | Less than                            | if (a < b) {}    |
| >=       | Greater than or equal to             | if (a >= b) {}   |
| <=       | Less than or equal to                | if (a <= b) {}   |
| &&       | Logical AND                          | if (a > 0 && b > 0) {} |
| \|\|     | Logical OR                           | if (a > 0 \|\| b > 0) {} |
| =        | Assignment                           | a = 10;          |
| +=       | Addition assignment                  | a += 5;          |
| -=       | Subtraction assignment               | b -= 3;          |
| *=       | Multiplication assignment            | c *= 2;          |
| /=       | Division assignment                  | d /= 4;          |
| %=       | Modulus assignment                   | e %= 3;          |

### If-else statements

If-else statements are used to make decisions in your code based on certain conditions. They allow you to execute different blocks of code depending on whether a condition is true or false.

The syntax for an if-else statement in C++ is as follows:

```cpp
if (condition) {
    // Code to execute if the condition is true
} else {
    // Code to execute if the condition is false
}
```

You can also use else-if statements to check multiple conditions:

```cpp
if (condition1) {
    // Code to execute if condition1 is true
} else if (condition2) {
    // Code to execute if condition2 is true
} else {
    // Code to execute if both conditions are false
}
```

Here is an example of an if-else statement in C++:

```cpp
#include <iostream>

using namespace std;

int main() {
    int age;
    cout << "Enter your age: ";
    cin >> age;

    if (age >= 18) {
        cout << "You are an adult." << endl;
    } else {
        cout << "You are a minor." << endl;
    }

    return 0;
}
```

In this example, we prompt the user to enter their age and store it in the `age` variable. We then use an if-else statement to check if the age is greater than or equal to 18. If the condition is true, we print "You are an adult." Otherwise, we print "You are a minor."

### Loops

Loops are used to execute a block of code repeatedly until a certain condition is met. In C++, there are three types of loops: for loops, while loops, and do-while loops.

#### For loops

A for loop is used when you know the number of iterations in advance. The syntax for a for loop in C++ is as follows:

```cpp
for (initialization; condition; increment/decrement) {
    // Code to execute in each iteration
}
```
Here is an example of a for loop in C++:

```cpp
#include <iostream>

using namespace std;

int main() {
    for (int i = 1; i <= 10; i++) {
        cout << i << " ";
    }
    cout << endl;
    return 0;
}
```

In this example, we use a for loop to print the numbers from 1 to 10. The loop initializes the variable `i` to 1, checks if `i` is less than or equal to 10, and increments `i` by 1 in each iteration. The code inside the loop prints the value of `i` followed by a space.

#### While loops

A while loop is used when you want to repeat a block of code as long as a certain condition is true. The syntax for a while loop in C++ is as follows:

```cpp
while (condition) {
    // Code to execute in each iteration
}
```

Here is an example of a while loop in C++:

```cpp
#include <iostream>

using namespace std;

int main() {
    int i = 1;
    while (i <= 10) {
        cout << i << " ";
        i++;
    }
    cout << endl;
    return 0;
}
```

In this example, we use a while loop to print the numbers from 1 to 10. The loop checks if `i` is less than or equal to 10, and if the condition is true, it prints the value of `i` followed by a space and increments `i` by 1.

#### Do-while loops

A do-while loop is similar to a while loop, but it guarantees that the code inside the loop will be executed at least once, even if the condition is false. The syntax for a do-while loop in C++ is as follows:

```cpp
do {
    // Code to execute in each iteration
} while (condition);
```

Here is an example of a do-while loop in C++:

```cpp
#include <iostream>

using namespace std;

int main() {
    int i = 1;
    do {
        cout << i << " ";
        i++;
    } while (i <= 10);
    cout << endl;
    return 0;
}
```

In this example, we use a do-while loop to print the numbers from 1 to 10. The code inside the loop prints the value of `i` followed by a space and increments `i` by 1. The loop then checks if `i` is less than or equal to 10, and if the condition is true, it repeats the process.

#### Break and continue statements

The `break` and `continue` statements are used to control the flow of loops in C++.

The `break` statement is used to exit a loop prematurely. When the `break` statement is encountered inside a loop, the loop is terminated, and the program continues with the next statement after the loop. Here is an example:

```cpp
#include <iostream>

using namespace std;

int main() {
    for (int i = 1; i <= 10; i++) {
        if (i == 5) {
            break; // Exit the loop when i is 5
        }
        cout << i << " ";
    }
    cout << endl;
    return 0;
}
```

In this example, the loop prints the numbers from 1 to 4. When `i` becomes 5, the `break` statement is executed, and the loop is terminated.

The `continue` statement is used to skip the current iteration of a loop and move to the next iteration. When the `continue` statement is encountered inside a loop, the remaining code in the current iteration is skipped, and the loop proceeds to the next iteration. Here is an example:

```cpp
#include <iostream>

using namespace std;

int main() {
    for (int i = 1; i <= 10; i++) {
        if (i % 2 == 0) {
            continue; // Skip even numbers
        }
        cout << i << " ";
    }
    cout << endl;
    return 0;
}
```

In this example, the loop prints only the odd numbers from 1 to 10. When `i` is an even number, the `continue` statement is executed, and the remaining code in that iteration is skipped.

### Functions

Functions are blocks of code that perform a specific task and can be reused throughout your program. They help to organize your code, make it more readable, and reduce redundancy.

The syntax for defining a function in C++ is as follows:

```cpp
return_type function_name(parameter1, parameter2, ...) {
    // Code to execute
    return value; // Optional, depending on the return type
}
```

Here is an example of a simple function in C++:

```cpp
#include <iostream>

using namespace std;

// Function to add two integers and return the result
int add(int a, int b) {
    return a + b;
}

int main() {
    int num1, num2;
    cout << "Enter two integers: ";
    cin >> num1 >> num2;

    // Call the add function and store the result
    int sum = add(num1, num2);
    cout << "The sum is: " << sum << endl;

    return 0;
}
```

In this example, we define a function named `add` that takes two integer parameters (`a` and `b`) and returns their sum. In the `main()` function, we prompt the user to enter two integers, call the `add` function with those integers as arguments, and store the result in the `sum` variable. Finally, we print the sum to the console.

### Arrays

An array is a collection of elements of the same data type that are stored in contiguous memory locations. Arrays allow you to store multiple values in a single variable and access them using an index.

The syntax for declaring an array in C++ is as follows:

```cpp
data_type array_name[array_size];
```

Here is an example of declaring and initializing an array in C++:

```cpp
#include <iostream>

using namespace std;

int main() {
    int numbers[5]; // Declare an array of 5 integers

    // Initialize the array
    numbers[0] = 10;
    numbers[1] = 20;
    numbers[2] = 30;
    numbers[3] = 40;
    numbers[4] = 50;

    // Access and print the elements of the array
    for (int i = 0; i < 5; i++) {
        cout << "Element at index " << i << ": " << numbers[i] << endl;
    }

    return 0;
}
```

In this example, we declare an array named `numbers` that can hold 5 integers. We then initialize the array by assigning values to each element using their respective indices. Finally, we use a for loop to access and print each element of the array.

You can also initialize an array at the time of declaration:

```cpp
int numbers[5] = {10, 20, 30, 40, 50}; // Declare and initialize an array
```

We can make it easier to work with arrays by using loops. For example, we can use a loop to initialize the array:

```cpp
int numbers[5]; // Declare an array of 5 integers

for (int i = 0; i < 5; i++) {
    numbers[i] = (i + 1) * 10; // Initialize the array with multiples of 10
}

// Access and print the elements of the array_size
for (int i = 0; i < 5; i++) {
    cout << "Element at index " << i << ": " << numbers[i] << endl;
}
```

In this modified example, we use a for loop to initialize the `numbers` array with multiples of 10. The loop iterates from 0 to 4, and in each iteration, it assigns the value `(i + 1) * 10` to the corresponding index of the array. This way, we can easily initialize the array without having to write multiple assignment statements.

We can also use `<vector>` from the Standard Template Library (STL) which is a dynamic array that can grow and shrink in size as needed. Here is an example of using a vector in C++:

```cpp
#include <iostream>
#include <vector>

using namespace std;

int main() {
    vector<int> numbers; // Declare a vector of integers

    // Add elements to the vector
    numbers.push_back(10);
    numbers.push_back(20);
    numbers.push_back(30);
    numbers.push_back(40);
    numbers.push_back(50);

    // Access and print the elements of the vector
    for (int i = 0; i < numbers.size(); i++) {
        cout << "Element at index " << i << ": " << numbers[i] << endl;
    }

    return 0;
}
```

In this example, we include the `<vector>` header and declare a vector named `numbers` that can hold integers. We use the `push_back` method to add elements to the vector. Finally, we use a for loop to access and print each element of the vector using the `size()` method to get the number of elements in the vector.

### Pointers

A pointer is a variable that stores the memory address of another variable. Pointers are used to directly access and manipulate memory, which can be useful for dynamic memory allocation, arrays, and functions.

The syntax for declaring a pointer in C++ is as follows:

```cpp
data_type* pointer_name;
```

Here is an example of declaring and using a pointer in C++:

```cpp
#include <iostream>

using namespace std;

int main() {
    int num = 42; // Declare an integer variable
    int* ptr = &num; // Declare a pointer and assign it the address of 'num'

    cout << "Value of num: " << num << endl; // Print the value of 'num'
    cout << "Address of num: " << &num << endl; // Print the address of 'num'
    cout << "Value of ptr: " << ptr << endl; // Print the value of 'ptr' (address of 'num')
    cout << "Value pointed to by ptr: " << *ptr << endl; // Dereference 'ptr' to get the value of 'num'

    *ptr = 100; // Change the value of 'num' using the pointer
    cout << "New value of num: " << num << endl; // Print the new value of 'num'

    return 0;
}
```

In this example, we declare an integer variable `num` and initialize it with the value 42. We then declare a pointer `ptr` and assign it the address of `num` using the address of operator (`&`). We print the value of `num`, its address, the value of `ptr` (which is the address of `num`), and the value pointed to by `ptr` (which is the value of `num`) using the dereference operator (`*`). Finally, we change the value of `num` to 100 using the pointer and print the new value.

### structures

A structure (struct) is a user-defined data type that allows you to group related variables of different data types into a single unit. Structures are useful for organizing complex data and creating custom data types.

The syntax for defining a structure in C++ is as follows:

```cpp
struct structure_name {
    data_type member1;
    data_type member2;
    // More members...
};
```

Here is an example of defining and using a structure in C++:

```cpp
#include <iostream>

using namespace std;

// Define a structure to represent a point in 2D space
struct Point {
    int x; // x-coordinate
    int y; // y-coordinate
};

int main() {
    Point p1; // Declare a variable of type Point

    // Initialize the members of the structure
    p1.x = 10;
    p1.y = 20;

    // Access and print the members of the structure
    cout << "Point p1: (" << p1.x << ", " << p1.y << ")" << endl;

    return 0;
}
```

In this example, we define a structure named `Point` that has two members: `x` and `y`, which represent the coordinates of a point in 2D space. In the `main()` function, we declare a variable `p1` of type `Point`, initialize its members, and print the coordinates of the point.

### Classes and Objects

A class is a user defined data type that serves as a blueprint for creating objects. It encapsulates data (attributes) and functions (methods) that operate on that data. Objects are instances of a class, and they can hold different values for the attributes defined in the class.

The syntax for defining a class in C++ is as follows:

```cpp
class class_name {
public:
    // Attributes (data members)
    data_type attribute1;
    data_type attribute2;
    // More attributes...

    // Methods (member functions)
    return_type method1(parameters) {
        // Code to execute
    }
    // More methods...
};
```

Here is an example of defining and using a class in C++:

```cpp
#include <iostream>

using namespace std;

// Define a class to represent a rectangle

class Rectangle {
public:
    // Attributes
    int width;
    int height;

    // Method to calculate the area of the rectangle
    int area() {
        return width * height;
    }
};

int main() {
    Rectangle rect; // Create an object of the Rectangle class

    // Initialize the attributes of the object
    rect.width = 10;
    rect.height = 5;

    // Call the area method and print the result
    cout << "Area of the rectangle: " << rect.area() << endl;

    return 0;
}
```

In this example, we define a class named `Rectangle` that has two attributes: `width` and `height`, and a method named `area()` that calculates the area of the rectangle. In the `main()` function, we create an object `rect` of the `Rectangle` class, initialize its attributes, and call the `area()` method to calculate and print the area of the rectangle.



