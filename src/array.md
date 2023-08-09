# Arrays And Strings
So, you know about variables, but have you wanted a list of variables in 1 variables? That's an array. An array is a variable that contains multiple variables. We we also cover what strings are.

## Declare an array
To declare an array, so simply do it similar to the variable declaration process. You do it like this:
```c
<const if const> <unsigned if unsigned> <type> <name>[<len>];
```
Type is the type, name is the name, and len is the length of the array. An example of this declration:
```c
unsigned int array_tape[5];
```
This array_tape is an array with length 5 and type unsigned int.

You can also set arrays:
```c
unsigned int array_tape[5] = {1, 2, 3, 4, 5};
```

## Accessing an array
In order to access an array member, you need to do this:
```c
<name>[<index>]
```
where name is the array name and index is a 0-indexed length.

### Wait, What? 0-indexed?
Yes, C is 0-indexed, which means in order to reach the 1st member of the array you need to do `array[0]`, the 2nd member `array[1]`, etc. This might seem weird and first, but you will get used to it.

## An example program using arrays
```c
#include <stdio.h>

int main() {
    unsigned int array[5] = {1, 3, 5, 7, 6};
    printf("Hello! Enter a 0-indexed index: ");
    int index = 0;
    scanf("%d", &index);
    printf("The value of array at %d: %d\n", index, array[index]);
}
```

## Strings
Strings are character arrays. Yeah, and they have a special format specifier: `%s`. `%s` simply prints the character array, like a string. Example:

```c
#include <stdio.h>

int main() 
    printf("%s", "Hello, World!\n");
    return 0;
}
```
This outputs `Hello, World!` with a newline like normal. To scan a string with scanf, you do this:

```c
#include <stdio.h>

int main() {
    // -- snip --
    char string[10];
    // notice we dont use a &.
    // this is because arrays have a special property that you don't need to worry about
    // right now
    scanf("%s", string);
    printf("%s\n", string);
}
```
