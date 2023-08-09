# Your First C Program
Alright, know let's start programming. First create a file, name it whatever you want. The extension must be `.c`, for example `hello.c`, `program.c`. Then type this into the file:

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

Now you can compile the C program:

```sh
$ # cd to the directory of the c file...
$ clang <cfile>
```
Replace `<cfile>` with your c file. Then you should see a file called `a.out` (linux, mac) or `a.exe` (windows). Run the executable, and...

```
Hello, World!
```
Wow! your first C program! Now let's explain what the code does.

```c
#include <stdio.h>
```
This includes the <b>St</b>andr<b>d</b> <b>I</b>nput/<b>O</b>utput header. This header contains functions for printing to the screen. The name `stdio.h` derives from `stdio`, which is short for standard input/output, and the `.h` part signifies this file is a header.

```c
int main() {
}
```
This is the main function for the program. When you run the program, this function is called. main returns an int, a number. 0 signifies success and 1 signifies failure. In this case for our hello world program it will never fail so we return 0.

```c
    printf("Hello, World!\n");
    return 0;
```
Note that the indentation is important. printf is a function that prints out the screen (with format). In this case we are printing `Hello, World!\n` where the `\n` part signifies add a newline, so that when we print twice it doesn't look like this:
```
Hello, World!Bye, World!
```
with a newline it looks like this:
```
Hello, World!
Bye, World!
```
Note that there is a return 0 statement, which means the program succeeded. Note there is also semicolons, and semicolons are kind of like the ending for the instruction to do. Think of it this way: `printf("Hello, World!\n")` is the instruction. So the semicolon means run it. So without the semicolon, the compiler wouldn't know if this is an instruction or not. This is a kind of complicated way to say it, so tl;dr there needs to be a semicolon after every line of code (excluding braces).

Keep in mind the brackets in the function: that means that make a new scope for the function instead of using the global scope. We will talk more about this later.
