# Libft
![42 School](https://img.shields.io/badge/-School-000000?style=flat-square&logo=42&logoColor=white) <br>
First C library project in the 42 curriculum: a custom libc-like library plus extra utilities and a linked-list bonus.  
Built with `-Wall -Wextra -Werror`, no global variables, and proper memory management (no leaks).

## Usage

```bash
make        # or make all
make clean
make fclean
make re
make bonus  # builds the linked-list functions too
```

## Functions

| Part | Function | Description |
|-----:|----------|-------------|
| Libc | `ft_isalpha` | Checks for an alphabetic character |
| Libc | `ft_isdigit` | Checks for a digit (0–9) |
| Libc | `ft_isalnum` | Checks for an alphanumeric character |
| Libc | `ft_isascii` | Checks whether `c` fits into the ASCII set |
| Libc | `ft_isprint` | Checks for any printable character |
| Libc | `ft_strlen` | Computes string length |
| Libc | `ft_memset` | Fills memory with a constant byte |
| Libc | `ft_bzero` | Sets a memory block to zero |
| Libc | `ft_memcpy` | Copies memory (no overlap safety) |
| Libc | `ft_memmove` | Copies memory (overlap-safe) |
| Libc | `ft_strlcpy` | Size-bounded string copy |
| Libc | `ft_strlcat` | Size-bounded string concatenation |
| Libc | `ft_toupper` | Lowercase → uppercase |
| Libc | `ft_tolower` | Uppercase → lowercase |
| Libc | `ft_strchr` | Finds first occurrence of a char in a string |
| Libc | `ft_strrchr` | Finds last occurrence of a char in a string |
| Libc | `ft_strncmp` | Compares two strings up to `n` bytes |
| Libc | `ft_memchr` | Scans memory for a byte |
| Libc | `ft_memcmp` | Compares memory areas |
| Libc | `ft_strnstr` | Finds a substring (size-bounded) |
| Libc | `ft_atoi` | Converts string to integer |
| Libc | `ft_calloc` | Allocates and zero-initializes (malloc) |
| Libc | `ft_strdup` | Duplicates a string (malloc) |
| Extra | `ft_substr` | Returns a substring (malloc) |
| Extra | `ft_strjoin` | Joins `s1` and `s2` (malloc) |
| Extra | `ft_strtrim` | Trims chars in `set` from start/end (malloc) |
| Extra | `ft_split` | Splits a string by a delimiter (malloc) |
| Extra | `ft_itoa` | Converts int to string (malloc) |
| Extra | `ft_strmapi` | Maps chars to a new string using `f` (malloc) |
| Extra | `ft_striteri` | Iterates chars, passing their address to `f` |
| Extra | `ft_putchar_fd` | Writes a char to a file descriptor |
| Extra | `ft_putstr_fd` | Writes a string to a file descriptor |
| Extra | `ft_putendl_fd` | Writes a string + `\n` to a file descriptor |
| Extra | `ft_putnbr_fd` | Writes an integer to a file descriptor |
| Bonus | `ft_lstnew` | Creates a new list node |
| Bonus | `ft_lstadd_front` | Adds a node at the beginning |
| Bonus | `ft_lstsize` | Counts list nodes |
| Bonus | `ft_lstlast` | Returns the last node |
| Bonus | `ft_lstadd_back` | Adds a node at the end |
| Bonus | `ft_lstdelone` | Deletes one node (uses `del` on content) |
| Bonus | `ft_lstclear` | Clears and frees the entire list |
| Bonus | `ft_lstiter` | Iterates list and applies `f` to content |
| Bonus | `ft_lstmap` | Applies `f` and creates a new list |

### Bonus: list struct

```c
typedef struct s_list
{
    void            *content;
    struct s_list   *next;
} t_list;
```
