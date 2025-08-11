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

Depending on your project configuration, bonus features might include:

- Support for additional format flags: `-`, `0`, `#`, ` `, and `+`
- Handling of field width and precision
- Support for printing to arbitrary file descriptors (e.g., `ft_dprintf`)
- Extended type handling or custom specifiers

Check the source code or project instructions for details on which bonuses are implemented.

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

## Contributing

Contributions are welcome! Feel free to open issues or pull requests.

## License

This project is open-source, distributed under the MIT License. See [LICENSE](LICENSE) for more information.
