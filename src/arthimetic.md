# Arithmetic and Everything fun
You know that in math you can add 2 numbers, subtract 2 numbers, etc. well in programming you can do the exact same things! In this entry we will cover over Arithmetic in C.

## This entry is quite short...
In fact you can sum up Arithmetic in just 1 C file, but for context: you can do Arithmetic on any C data type. So, we can make a simple calculator.

```c
#include <stdio.h>

int main() {
    float op1 = 0.0f;
    float op2 = 0.0f;
    printf("Calculator (TM)\n");
    printf("Enter 2 numbers:\n");
    scanf("%f", &op1);
    scanf("%f", &op2);
    // addition
    printf("%f + %f = %f\n", op1, op2, op1 + op2);
    // subtraction
    printf("%f - %f = %f\n", op1, op2, op1 - op2);
    // multiplication
    printf("%f * %f = %f\n", op1, op2, op1 * op2);
    // division
    printf("%f / %f = %f\n", op1, op2, op1 / op2);
    // for short you can do Arithmetic on any c type and literal
    // you can do int a = b + 5; etc
    // this is a very short entry...... very simple
    printf("Bye!\n");
    return 0;
}
```
