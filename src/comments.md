# Comments & Escape Sequences
Alright, so know you know how to make a hello world program and use printf, lets cover more things.

## Comments
Comments can be used to describe your code, signfiy stuff, maybe a todo? Whatever, comments are like sticky notes for code. Let's see an example of comments:

```c
#include <stdio.h>

int main() {
    // This is a comment
    /*
        This
        is
        a
        multiline
        comment
    */
    printf("Hello, World!\n");
    return 0;
}
```
There are 2 types of comments: single-line comments (`//`) and multi-line comments (`/* */`).

Single-line comments are, single-line comments. Multiline comments are single-line comments but they can span multiple lines. Oh, and multiline comments start with `/*` and end with `*/`. Yeah so that's comments.

## Escape Sequences
Now this is the fun part. In the hello world program, remember that I said the `\n` was a newline. `\n` is a escape sequence that means print newline. There are also more escape sequences, which i'll talk about.

### \n
Newline - prints a newline
```c
#include <stdio.h>

int main() {
    printf("Hello!\n");
    printf("Bye!\n");
    return 0;
}
```
Output:
```
Hello!
Bye!
```
### \t
Tab - prints a tab (aka long space, indent)
```c
#include <stdio.h>

int main() {
    printf("1\t2\t3\n");
    return 0;
}
```
Output:
```
1   2   3
```

### \\"
This one is complicated. This exists because you can't enter `"` in a printf as `"` starts and ends the string. so you use `\"` in printf to print out the `"`
```c
#include <stdio.h>

int main() {
    printf("\"blah blah I eat something\" - me, 2023 (not colorized)");
    return 0;
}
```
Output:
```
"blah blah I eat something" - me, 2023 (not colorized)
```

## That's most of the escape sequeneces you need to know
There are more but you don't use them a lot. So that's it for this entry.

```c
#include <stdio.h>

int main() {
    printf("Bye!\n");
    return 0;
}
```
