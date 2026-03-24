# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 29/01/2026
# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof() :
  
   3.1 Integer literal (e.g., 10) using `%d`
   
   3.2 Float literal (e.g., 3.14) using `%f`
   
   3.3 Character literal (e.g., 'A') using `%c`
   
   3.4 String literal (e.g., "Hello C") using `%s`
   
### Step 4: 
   Stop
# Program:
```
#include <stdio.h>

int main() {
    int number = 10;
    float price = 25.5;
    char letter = 'C';
    char text[] = "Welcome to C";
    printf("Integer value: %d\n", number);
    printf("Float value: %.1f\n", price);
    printf("Character value: %c\n", letter);
    printf("String value: %s\n", text);

    return 0;
}
```
# Output:
<img width="501" height="417" alt="image" src="https://github.com/user-attachments/assets/384e4766-3106-43f3-97c5-8a1403024a7a" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 29/1/2026
# Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
# Algorithm:
### Step 1:
  Start  
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Define a macro constant `PI` with value `3.14159` using `#define`.
### Step 4: 
   Inside `main()`:
   
   4.1 Declare a constant integer variable `DAYS`
   
   4.2 Initialize it with the value `7`
   
### Step 5:  
  Use `printf()` to display the values of `PI` and `DAYS`.     
### Step 6:  
  Stop
# Program:
```
#include <stdio.h>
#define MAX 100
int main() {
    const int MIN = 10;
    printf("Macro constant MAX = %d\n", MAX);
    printf("Constant variable MIN = %d\n", MIN);
    return 0;
}
```
# Output:
<img width="535" height="324" alt="image" src="https://github.com/user-attachments/assets/26daf362-9ef5-4272-8c92-0caae0d687b0" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 
# Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside main(), declare and initialize variables of types int, float, double, and char.
### Step 4: 
   Display their values using printf().
### Step 5:    
   Stop
# Program:
```
#include <stdio.h>
int main() {
    int count = 10;           
    float price = 25.75f;     
    double distance = 123.456; 
    char grade = 'A';         
    printf("Integer value: %d\n", count);
    printf("Float value: %.2f\n", price);
    printf("Double value: %.3lf\n", distance);
    printf("Character value: %c\n", grade);
    return 0;
}
```
# Output:
<img width="466" height="365" alt="image" src="https://github.com/user-attachments/assets/35e9ce1b-d95e-4dc3-8781-ada17063f9f5" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.
# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 
# Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare two integer variables a and b.
### Step 4: 
   Prompt the user to enter two integers and read the input using scanf().
### Step 5:    
   Perform arithmetic operations on a and b:
   #### Sum (a + b)
   #### Difference (a - b)
   #### Product (a * b)
   #### Quotient (a / b)
   #### Remainder (a % b)
### Step 6: 
  Perform bitwise operations on a and b:
  #### AND (a &amp; b)
  #### OR (a | b)
  #### XOR (a ^ b)
  #### Left shift (a << b)
  #### Right shift (a >> b)
  #### Bitwise NOT of a (~a) and b (~b)
### Step 7:   
  Display the results of all operations using printf().
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>

int main() {
    int a, b;
    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);
    printf("\nArithmetic Operations:\n");
    printf("Addition (a + b): %d\n", a + b);
    printf("Subtraction (a - b): %d\n", a - b);
    printf("Multiplication (a * b): %d\n", a * b);

    if (b != 0) {
        printf("Division (a / b): %d\n", a / b);
        printf("Remainder (a %% b): %d\n", a % b);
    } else {
        printf("Division and Remainder not possible (division by zero)\n");
    }
    printf("\nBitwise Operations:\n");
    printf("AND (a & b): %d\n", a & b);
    printf("OR (a | b): %d\n", a | b);
    printf("XOR (a ^ b): %d\n", a ^ b);
    printf("Left Shift (a << 1): %d\n", a << 1);
    printf("Right Shift (a >> 1): %d\n", a >> 1);
    printf("NOT (~a): %d\n", ~a);

    return 0;
}
```
# Output:
<img width="348" height="488" alt="image" src="https://github.com/user-attachments/assets/3e2a72f8-790e-4d3d-b588-0b9d3ad8bb5c" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 
# Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Input a character ch from the user.
### Step 4: 
   Check if ch is a digit ('0' to '9').
   
   If true → Print "Digit" → Go to Step 8.
   
   If false → Go to Step 5.
   
### Step 5:    
   Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').
   
   If true → Go to Step 6.
   
   If false → Go to Step 7.
   
### Step 6: 
   Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).
   
   If true → Print "Vowel" → Go to Step 8.
   
   If false → Print "Consonant" → Go to Step 8.
   
### Step 7:   
   Print "Special Symbol".
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>
int main() {
    char ch;
    printf("Enter a character: ");
    scanf("%c", &ch);
    (ch >= '0' && ch <= '9') ?
        printf("The character is a Digit.\n") :
    ((ch >= 'A' && ch <= 'Z') || (ch >= 'a' && ch <= 'z')) ?
        ((ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U' ||
          ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u') ?
            printf("The character is a Vowel.\n") :
            printf("The character is a Consonant.\n")) :
        printf("The character is a Special Symbol.\n");
    return 0;
}
```
# Output:
<img width="544" height="365" alt="image" src="https://github.com/user-attachments/assets/e5f5199c-9f3e-4364-ac10-5faf9bfce9e0" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


