# ft_printf

Remake of the standard C `printf` function, with additional bonuses.

> **Note:** This project is the official [42 school](https://42.fr) `ft_printf` project.

## Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Supported Format Specifiers](#supported-format-specifiers)
- [Bonus Features](#bonus-features)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## About the Project

`ft_printf` is a custom implementation of the C standard library function `printf`. The goal of this project is to reproduce the behavior of `printf` as closely as possible, handling formatted output with various data types, and to extend its functionality with some bonus features.

This project was built as part of the **42 school curriculum**. It is a required core project at 42, designed to teach students variadic functions, parsing, and low-level output in C.

## Features

- Handles formatted output for characters, strings, integers, unsigned integers, hexadecimal, pointers, and the `%` character.
- Supports flags, width, and precision modifiers (as per standard `printf`).
- Includes bonus features (see below).
- Written in pure C (C99 standard).

## Supported Format Specifiers

| Specifier | Description             |
|-----------|------------------------|
| `%c`      | Character              |
| `%s`      | String                 |
| `%p`      | Pointer address        |
| `%d`      | Signed integer         |
| `%i`      | Signed integer         |
| `%u`      | Unsigned integer       |
| `%x`      | Lowercase hexadecimal  |
| `%X`      | Uppercase hexadecimal  |
| `%%`      | Percent sign           |

## Bonus Features

The bonus part of the 42 ft_printf project includes support for the following flags and features, which can be used in any combination:

| Flag        | Description                                                                |
|-------------|----------------------------------------------------------------------------|
| `-`         | Left-justify within the given field width                                  |
| `0`         | Pad with zeros instead of spaces                                           |
| `.`         | Precision specification (e.g., `.5`)                                       |
| (width)     | Field minimum width (e.g., `10` for a width of 10)                         |
| `#`         | Use alternative form (`0x`, `0X`, or `0` prefix for hex/oct, as applicable)|
| ` ` (space) | Prefix a space for positive numbers in signed conversions                  |
| `+`         | Always prefix a sign (`+` or `-`) for signed conversions                   |

> **Note:** The bonus part requires you to manage any combination of the flags `'-'`, `'0'`, `'.'`, and the field minimum width under all conversions, and to fully support the `'#'`, `' '`, and `'+'` flags.

## Project Structure

```
ft_printf/
├── Makefile
├── ft_printf.c
├── ft_printf.h
├── (other .c/.h source files)
```

- `ft_printf.c`: Main implementation of the `ft_printf` function.
- `ft_printf.h`: Header file with function prototypes.
- Other `.c`/`.h` files: Helpers and bonus feature implementations.

## License

This project is part of the 42 school curriculum and is intended for educational purposes.
