---

# Libft

Libft is a custom implementation of essential standard library functions for the C programming language. This project provides commonly used utility functions for `string`, `memory`, and `linked list` operations, along with additional helper functions. Libft serves as a foundational library for developing more complex C projects.

## Features

- **String Manipulation**: Functions like `ft_strlen`, `ft_strdup`, `ft_strjoin`, and `ft_split` enable efficient text processing.
- **Memory Management**: Use functions such as `ft_memset`, `ft_memcpy`, `ft_bzero`, and `ft_calloc` for memory operations.
- **Character Classification**: Functions like `ft_isalpha`, `ft_isdigit`, `ft_tolower`, and `ft_toupper` help handle character-based data.
- **Linked List Management**: Provides utilities like `ft_lstnew`, `ft_lstadd_back`, and `ft_lstmap` to simplify dynamic data structures.

## Installation

Clone the repository and build the library:

```bash
git clone https://github.com/username/libft.git
cd libft
make
```

This will generate a static library file `libft.a` that you can link to your C projects.

## Usage

To use Libft in your project, include `libft.h` and link the `libft.a` file during compilation. For example:

```bash
gcc main.c -L. -lft -o my_program
```

Here, `main.c` is your program's main file, `-L.` specifies the directory containing `libft.a`, and `-lft` links the library.

## Example

```c
#include "libft.h"
#include <stdio.h>

int main(void) {
    char *message = ft_strdup("Welcome to Libft!");
    printf("%s\n", message);
    free(message);

    int number = 42;
    char *num_str = ft_itoa(number);
    printf("Number: %s\n", num_str);
    free(num_str);

    return 0;
}
```

## Contributing

Contributions are welcome! If you encounter any issues or have ideas for improvement, feel free to open an issue or submit a pull request.
