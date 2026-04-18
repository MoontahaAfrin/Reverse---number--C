# Reverse---number--C
C program to reverse a number
# Reverse Number in C

##  Problem
Write a C program to reverse the digits of a given number.

##  Explanation
This program takes an integer as input and reverses its digits using a loop. 
Each digit is extracted using modulus (%) and added to the reversed number.

## 💻 Code
```c
#include <stdio.h>

int main() {
    int n, reverse = 0, remainder;

    printf("Enter a number: ");
    scanf("%d", &n);

    while(n != 0) {
        remainder = n % 10;
        reverse = reverse * 10 + remainder;
        n = n / 10;
    }

    printf("Reversed number = %d", reverse);

    return 0;
}
