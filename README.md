# 📚 LibFT - My Custom C Library

![42 Badge](https://img.shields.io/badge/42-School-000000?style=flat-square&logo=42&logoColor=white)
![C Badge](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)

> *"The foundation of all great software begins with solid fundamentals."*

Welcome to **LibFT**, my personal implementation of essential C library functions! This project represents the cornerstone of my journey at 42 School, where I rebuilt fundamental C library functions from scratch to gain deep understanding of memory management, string manipulation, and algorithmic thinking.

## 🌟 What Makes This Special

LibFT isn't just another C library – it's a testament to understanding computing fundamentals at the lowest level. Every function has been meticulously crafted following 42 School's rigorous coding standards, emphasizing:

- **Memory Safety**: Bulletproof memory management with no leaks
- **Code Quality**: Clean, readable, and maintainable code
- **Performance**: Optimized algorithms with careful attention to efficiency
- **Reliability**: Thoroughly tested edge cases and error handling

## 🛠️ Function Categories

### 🔤 Character Classification & Conversion
Functions that analyze and transform individual characters:
```c
ft_isalpha()    // Check if character is alphabetic
ft_isdigit()    // Check if character is numeric
ft_isalnum()    // Check if character is alphanumeric
ft_isascii()    // Check if character is ASCII
ft_isprint()    // Check if character is printable
ft_toupper()    // Convert to uppercase
ft_tolower()    // Convert to lowercase
```

### 🧠 Memory Management
Low-level memory manipulation functions:
```c
ft_memset()     // Fill memory with constant byte
ft_memcpy()     // Copy memory area
ft_memmove()    // Copy memory area (overlap-safe)
ft_memchr()     // Scan memory for character
ft_memcmp()     // Compare memory areas
ft_bzero()      // Zero out memory
ft_calloc()     // Allocate and zero memory
```

### 🔧 String Manipulation
Comprehensive string handling utilities:
```c
ft_strlen()     // Calculate string length
ft_strchr()     // Locate character in string
ft_strrchr()    // Locate character in string (reverse)
ft_strncmp()    // Compare strings
ft_strnstr()    // Locate substring
ft_strlcpy()    // Safe string copy
ft_strlcat()    // Safe string concatenation
ft_strdup()     // Duplicate string
```

### ✨ Advanced String Operations
High-level string processing functions:
```c
ft_substr()     // Extract substring
ft_strjoin()    // Join two strings
ft_strtrim()    // Trim characters from string
ft_split()      // Split string by delimiter
ft_strmapi()    // Apply function to each character
ft_striteri()   // Apply function to each character (with index)
```

### 🔢 Conversion & I/O
Data conversion and output functions:
```c
ft_atoi()       // String to integer conversion
ft_itoa()       // Integer to string conversion
ft_putchar_fd() // Output character to file descriptor
ft_putstr_fd()  // Output string to file descriptor
ft_putendl_fd() // Output string with newline to fd
ft_putnbr_fd()  // Output number to file descriptor
```

### 🔗 Linked List Operations (Bonus)
Complete linked list manipulation toolkit:
```c
ft_lstnew()       // Create new list element
ft_lstadd_front() // Add element at beginning
ft_lstadd_back()  // Add element at end
ft_lstsize()      // Count list elements
ft_lstlast()      // Get last element
ft_lstdelone()    // Delete single element
ft_lstclear()     // Delete entire list
ft_lstiter()      // Apply function to each element
```

## 🚀 Quick Start

### Prerequisites
- GCC compiler
- Make utility
- Unix-like operating system (Linux/macOS)

### Installation
```bash
# Clone the repository
git clone https://github.com/Myxoceph/Libft libft
cd libft

# Compile the library
make

# For bonus functions
make bonus

# Clean object files
make clean

# Full cleanup
make fclean
```

### Usage Example
```c
#include "libft.h"
#include <stdio.h>

int main(void)
{
    char *str = ft_strdup("Hello, World!");
    char **words = ft_split(str, ' ');
    
    printf("Original: %s\n", str);
    printf("First word: %s\n", words[0]);
    printf("Length: %zu\n", ft_strlen(str));
    
    // Clean up memory
    free(str);
    // Free words array...
    
    return (0);
}
```

## 🏗️ Project Structure
```
libft/
├── 📄 Makefile           # Build configuration
├── 📄 libft.h            # Header file with all prototypes
├── 📄 README.md          # This file
├── 🔧 ft_*.c             # Core function implementations
└── 🎁 ft_*_bonus.c       # Bonus linked list functions
```

## ✅ Technical Highlights

- **Norm Compliant**: All code follows 42 School's strict coding standards
- **No Standard Library**: Built from scratch without using standard C library functions
- **Memory Safe**: Proper memory allocation and deallocation practices
- **Edge Case Handling**: Comprehensive error checking and boundary condition management
- **Modular Design**: Each function is independent and reusable

## 🎯 Skills Demonstrated

This project showcases proficiency in:
- **Low-level Programming**: Direct memory manipulation and pointer arithmetic
- **Algorithm Design**: Efficient implementation of classic algorithms
- **Code Quality**: Writing clean, maintainable, and well-documented code
- **Testing**: Thorough testing and debugging practices
- **Build Systems**: Makefile creation and dependency management

## 🧪 Testing

All functions have been rigorously tested with:
- Unit tests for individual functions
- Edge case verification
- Memory leak detection with Valgrind
- Performance benchmarking

## 🤝 Contributing

This is an educational project from 42 School. While direct contributions aren't accepted, I'm always open to feedback and discussions about implementation approaches!

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🙋‍♂️ About the Developer

I'm a passionate software engineer who believes in understanding technology from the ground up. This LibFT project represents my commitment to mastering fundamentals before building on top of them. Every line of code here has been written with care, attention to detail, and a deep respect for the craft of programming.

---

*Built with ❤️ at 42 School - Where we don't just learn to code, we learn to think.*
