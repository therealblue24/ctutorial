# Variables
Now let's get into variables.

If you're asking "What are variables?" Well, if you went to pre-algebra, variables are kind of like math variables. They hold a value. However, variables in programming can have types. Let's get into it.

## Variable types
There are 3 core variable types:
* integer - number that has no decimal (short, int, long)
* floating point number - number that has a decimal (float, double)
* character - a character (char)

Types can be signed or unsigned, that is, they can be negative (signed) or never negative (unsigned). Integers can be signed and unsigned, floating point numbers are always signed, and characters can be signed and unsigned.

## Declaring a variable
Declaring a variable is easy. You do it like this:
```c
<unsigned if unsigned> <type> <name>;
```
Where you replace type with a variable type, and name with the variable name. Example:
```c
unsigned int tardy; // always >=0, number 
float gpa; // A gpa is in the range of 0.0 - 4.0, so float
char grade; // A grade is A-F, so a character
```
## Assigning a value to a variable
Assigning a value to a variable is also easy. You do it like this:
```c
<name> = <val>;
```
where you replace name with the variable name and val with the value to assign it to. Example:
```c
unsigned int tardy; // always >=0, number 
float gpa; // A gpa is in the range of 0.0 - 4.0, so float
char grade; // A grade is A-F, so a character
tardy = 2; // 2 tardys
gpa = 3.5f; // gpa is 3.5, notice the f at the end that means this value is a floating point
grade = 'B'; // a character has single quotes, '' while a string has double quotes ""
```

## Declaring and Assigning a value to a variable
You can do 2 at once. You do it like this:
```c
<unsigned if unsigned> <type> <name> = <val>;
```
This is easy. An example:
```c
unsigned int tardy = 2; // always >=0, number, 2 tardys
float gpa = 3.5f; // A gpa is in the range of 0.0 - 4.0, so float & gpa is 3.5, notice the f at the end that means this value is a floating point
char grade = 'B'; // A grade is A-F, so a character & a character has single quotes, '' while a string has double quotes ""
```
There is also constant variables, which you apply const before the variable declaraction. Constant variables never change. Example:
```c
const unsigned int hours_of_school = 7; // hours_of_school is always 7.
```
## Extra: format specifier for printf
You can print variables using format specifiers! Example:
```c
#include <stdio.h>

int main() {
    int hours_of_school = 7;
    // %d is the specifier for the int type
    // we also pass in hours_of_school to printf
    printf("Hours of school: %d\n", hours_of_school);
    hours_of_school = 0;
    // You can reassign and then print again. Summer is amazing by the way.
    printf("Hours of school in summer: %d\n", hours_of_school);
    return 0;
}
```
Here is the table of formats to use:

| Type  | Specifier   |
|-------------- | -------------- |
| int    | %d |
| long | %ld |
| short | %h |
| char  | %c |
| unsigned int | %u |
| unsigned long | %lu |
| unsigned short | %hu |
| unsigned char  | %c |
| float | %f |
| double | %lf |

## And now you know variables!
And format specifiers :)
```c
#include <stdio.h>

int main() {
    printf("Bye!\n");
    return 0;
}
```
