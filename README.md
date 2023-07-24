# Custom _printf Project

## Table of Contents
1. [Description](#description)
2. [How to Use](#how-to-use)
3. [Supported Conversion Specifiers](#supported-conversion-specifiers)
4. [Function Descriptions](#function-descriptions)
5. [Example Usage](#example-usage)
6. [Contributing](#contributing)
7. [License](#license)

## Description
The Custom _printf project is an implementation of the standard C library function `printf`, which is used for formatted output to the standard output stream. This custom version, `_printf`, provides similar functionality to the standard `printf` function and supports various format specifiers.

## How to Use
To use the custom `_printf` function in your C code, follow these steps:
1. Include the "holberton.h" header file in your C source file.
2. Call the `_printf` function in your code with the desired format string and arguments.

## Supported Conversion Specifiers
The custom `_printf` function supports the following conversion specifiers:
- `%c` : Character
- `%s` : String
- `%i` or `%d` : Integer (signed decimal)
- `%u` : Unsigned Integer (unsigned decimal)
- `%o` : Octal
- `%x` : Hexadecimal (lowercase)
- `%X` : Hexadecimal (uppercase)
- `%r` : Reverse the string (Rot13 encoding)
- `%b` : Binary
- `%R` : Rot13 encoding

## Function Descriptions
1. `int _printf(const char *format, ...)`: This is the main function for formatted output. It takes a format string `format` and optional arguments, similar to `printf`.

2. `int print_char(va_list c, int width)`: Prints a character from the `va_list` with optional left justification using the `-` flag and field width.

3. `int print_string(va_list s, int width)`: Prints a string from the `va_list` with optional left justification using the `-` flag and field width.

4. `int print_int(va_list i, int width)`: Prints a signed integer from the `va_list` with optional left justification using the `-` flag and field width.

5. `int print_unsigned(va_list u, int width)`: Prints an unsigned integer from the `va_list` with optional left justification using the `-` flag and field width.

6. `int print_octal(va_list o, int width)`: Prints an octal number from the `va_list` with optional left justification using the `-` flag and field width.

7. `int print_hex(va_list x, int width)`: Prints a hexadecimal number (lowercase) from the `va_list` with optional left justification using the `-` flag and field width.

8. `int print_rot13(va_list R, int width)`: Prints a string in Rot13 encoding from the `va_list` with optional left justification using the `-` flag and field width.

9. `int print_binary(va_list b, int width)`: Prints a binary number from the `va_list` with optional left justification using the `-` flag and field width.

## Example Usage
```c
#include "main.h"
#include <stdio.h>

int main(void)
{
    char *name = "John";
    int age = 25;

    _printf("Name: %-10s, Age: %d\n", name, age);

    return (0);
}
