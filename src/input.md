# Getting User Input
Alright, now let's actually get input from the user. Using a new function!
This is quite a short entry.

## scanf
scanf is kind of like printf (it has format specifiers) but it does the opposite function: it takes in user input.

So let's use it!

```c
// scanf is part of stdio
#include <stdio.h>

int main() {
    // variable
    int user_input = 0;
    // prompt
    printf("Hello! Please enter a number: ");
    // scanf
    // %d is the specifier for int
    // we add the & to user_input for reasons that you don't need to deal with now
    scanf("%d", &user_input);
    // user has inputted the number
    printf("\nYou entered: %d\n", user_input);
    return 0;
}
```
Compile this program and enter a number. You should see that the program outputs the number you entered. Amazing!

You can do this with any C type (int, short, long, float, etc.)

So yeah. That's scanf. Very useful.

```c
#include <stdio.h>

int main() {
    printf("Bye!\n");
    return 0;
}
```
