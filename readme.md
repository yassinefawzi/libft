📚 Libft — 42/1337 C Standard Library
<p align="center"> <img src="https://img.shields.io/badge/School-42/1337-blue?style=for-the-badge" /> <img src="https://img.shields.io/badge/Language-C-00599C?style=for-the-badge&logo=c&logoColor=white" /> <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" /> <img src="https://img.shields.io/badge/Norm-42_Norm-2ea44f?style=for-the-badge" /> </p>
🌟 Overview

Libft is the first project in the 42/1337 Network.
The goal is to recreate a custom C standard library, implementing essential functions from <ctype.h>, <string.h>, <stdlib.h>, and more — all written from scratch, following the strict 42 Norm.

This library will later serve as the foundation for many 42 projects.

✨ Features

🧠 Reimplementation of standard C library functions

🧵 Memory, strings, arrays, conversions

🏗️ A complete linked-list API (Bonus)

⚙️ Fully norm-compliant

📦 Delivered as a static library: libft.a

📁 Project Structure
libft/
├── ft_*.c
├── libft.h
├── Makefile
└── README.md


After compilation:

libft.a

📌 Part 1 — Libc Functions
🔤 Character checks

ft_isalpha — ft_isdigit — ft_isalnum — ft_isascii — ft_isprint

🧠 Memory

ft_memset — ft_bzero — ft_memcpy — ft_memmove — ft_memchr — ft_memcmp

🧵 Strings

ft_strlen — ft_strlcpy — ft_strlcat — ft_strchr — ft_strrchr — ft_strncmp — ft_strnstr

🔄 Conversions

ft_atoi — ft_toupper — ft_tolower

🏗️ Memory Allocation

ft_calloc — ft_strdup

💎 Part 2 — Additional Functions

✂️ ft_substr — Extract substring

➕ ft_strjoin — Concatenate strings

✨ ft_strtrim — Trim characters

🪓 ft_split — Split by delimiter

🔁 ft_strmapi, ft_striteri — Map/iterate string

🔢 ft_itoa — Integer to ASCII

📤 File descriptor output:
ft_putchar_fd, ft_putstr_fd, ft_putendl_fd, ft_putnbr_fd

🧩 Bonus — Linked List Functions

If bonus is completed:

ft_lstnew

ft_lstadd_front

ft_lstsize

ft_lstlast

ft_lstadd_back

ft_lstdelone

ft_lstclear

ft_lstiter

ft_lstmap

<p align="center"> <img src="https://img.shields.io/badge/Bonus-Included-9cf?style=for-the-badge" /> </p>
🔧 Compilation

Use the Makefile:

make         # compile libft.a
make clean   # remove *.o
make fclean  # remove *.o + libft.a
make re      # rebuild everything

🧪 Testing
🔎 Compile with your own main:
cc main.c -L. -lft

🧰 Recommended external testers:
Tester	Description
🐙 Libft-Unit-Test	Unit tests for all functions
🧪 libft-war-machine	Stress tests & error detection
🔥 Moulinette (francinette)	Official testing tool

(Not included in the repo — clone them separately.)

📜 Requirements

✔️ Follow the 42 Norm
✔️ No memory leaks
✔️ No segmentation faults
✔️ Clean and modular code
✔️ Only allowed functions: write, malloc, free

🎯 Learning Objectives

Understand low-level memory management

Gain mastery over strings and pointers

Build solid foundations for all future 42 projects

Write maintainable, reusable C code

Learn to work under strict norms & constraints

🚀 Example Usage
#include "libft.h"
#include <stdio.h>

int main(void)
{
    char *s = ft_strdup("Hello Libft!");
    printf("%s\n", s);
    free(s);
}


Compile:

cc test.c -L. -lft

📝 Author

👤 Yassine Fawzi
📍 1337/42 Network yfawzi
📧 fawziy217@gmail.com
