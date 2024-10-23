# 0x00. Python - Hello, World

## Author's disclaimer

```sh
Welcome to the Python world!

The first projects are more "C-oriented" - no tricks, no funky syntax - simple!
If you've already played with Python, don't worry, fun things will come.
You'll soon find that with Python (and the majority of higher level languages), there are ten different ways to do the same thing. Some tasks will expect only one implementation, while other tasks will have multiple possible implementations.
Like C, Python also has a linter / style guide like Betty, called PEP8, also now known as PyCode.

Enjoy!

- Guillaume
```

## Resources

- [The Python Tutorial](https://docs.python.org/3/tutorial/index.html) (Only the first three chapters below)
- [Whetting your appetite](https://docs.python.org/3/tutorial/appetite.html)
- [Using the Python Interpreter](https://docs.python.org/3/tutorial/interpreter.html)
- [An informal Introduction into Python](https://docs.python.org/3/tutorial/introduction.html) (Read up until '3.1.2. Strings')
- [How To Use String Formatters in Python 3](https://realpython.com/python-f-strings/)
- [Learn to Program](https://www.youtube.com/playlist?list=PLGLfVvz_LVvTn3cK5e6LjhgGiSeVlIRwt)
- [Pycodestyle – Style Guide for Python Code](https://pypi.org/project/pycodestyle/)

## Learning Objectives

### General

- Why Python programming is awesome
- Who created Python
- Who is Guido van Rossum
- Where does the name ‘Python’ come from
- What is the Zen of Python
- How to use the Python interpreter
- How to print text and variables using `print`
- How to use strings
- What are indexing and slicing in Python
- What is the official Python coding style and how to check your code with `pycodestyle`

### Copyright - Plagiarism

- You are tasked to come up with solutions for the tasks below yourself to meet with the above learning objectives.
- You will not be able to meet the objectives of this or any following project by copying and pasting someone else’s work.
- You are not allowed to publish any content of this project.
- Any form of plagiarism is strictly forbidden and will result in removal from the program.

## Requirements

### Python Scripts

- Allowed editors: vi, vim, emacs
- All your files will be interpreted/compiled on Ubuntu 20.04 LTS using python3 (version 3.8.5)
- All your files should end with a new line
- The first line of all your files should be exactly `#!/usr/bin/python3`
- A `README.md` file at the root of the repo, containing a description of the repository
- A `README.md` file, at the root of the folder of this project, is mandatory
- Your code should use the pycodestyle (version 2.8.*)
- All your files must be executable
- The length of your files will be tested using `wc`

### Shell Scripts

- Allowed editors: vi, vim, emacs
- All your scripts will be tested on Ubuntu 20.04 LTS
- All your scripts should be exactly two lines long (`wc -l file` should print 2)
- All your files should end with a new line
- The first line of all your files should be exactly `#!/bin/bash`
- All your files must be executable

### C Scripts

- Allowed editors: vi, vim, emacs
- All your files will be compiled on Ubuntu 20.04 LTS using gcc, using the options `-Wall -Werror -Wextra -pedantic -std=gnu89`
- All your files should end with a new line
- Your code should use the Betty style. It will be checked using `betty-style.pl` and `betty-doc.pl`
- You are not allowed to use global variables
- No more than 5 functions per file
- In the following examples, the `main.c` files are shown as examples. You can use them to test your functions, but you don’t have to push them to your repo (if you do we won’t take them into account). We will use our own `main.c` files at compilation. Our `main.c` files might be different from the one shown in the examples
- The prototypes of all your functions should be included in your header file called `lists.h`
- Don’t forget to push your header file
- All your header files should be include guarded

## More Info

### Zen
```
The Zen of Python, by Tim Peters

Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
Flat is better than nested.
Sparse is better than dense.
Readability counts.
Special cases aren't special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one-- and preferably only one --obvious way to do it.
Although that way may not be obvious at first unless you're Dutch.
Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it's a bad idea.
If the implementation is easy to explain, it may be a good idea.
Namespaces are one honking great idea -- let's do more of those!
```

### Pycodestyle
`Pycodestyle` is now the new standard of Python style code

## Quiz Questions

### 0. Run Python File

Write a Shell script that runs a Python script.

The Python file name will be saved in the environment variable `$PYFILE`

```sh
guillaume@ubuntu:~/py/0x00$ cat main.py 
#!/usr/bin/python3
print("Best School")

guillaume@ubuntu:~/py/0x00$ export PYFILE=main.py
guillaume@ubuntu:~/py/0x00$ ./0-run
Best School
guillaume@ubuntu:~/py/0x00$ 
```

**Repo**:

- GitHub repository: `alx-higher_level_programming`
- Directory: `0x00-python-hello_world`
- File: `0-run`

### 1. Run Inline

Write a Shell script that runs Python code.

The Python code will be saved in the environment variable `$PYCODE`

```sh
guillaume@ubuntu:~/py/0x00$ export PYCODE='print(f"Best School: {88+10}")'
guillaume@ubuntu:~/py/0x00$ ./1-run_inline 
Best School: 98
guillaume@ubuntu:~/py/0x00$ 
```

**Repo**:

- GitHub repository: `alx-higher_level_programming`
- Directory: `0x00-python-hello_world`
- File: `1-run_inline`

### 2. Hello, print

Write a Python script that prints exactly `"Programming is like building a multilingual puzzle,` followed by a new line.

- Use the function print

```sh
guillaume@ubuntu:~/py/0x00$ ./2-print.py 
"Programming is like building a multilingual puzzle
guillaume@ubuntu:~/py/0x00$
```

**Repo**:

- GitHub repository: `alx-higher_level_programming`
- Directory: `0x00-python-hello_world`
- File: `2-print.py`

### 3. Print integer

Complete this [source code](https://github.com/alx-tools/0x00.py/blob/master/3-print_number.py) in order to print the integer stored in the variable `number`, followed by `Battery street`, followed by a new line.

- You can find the source code [here](https://github.com/alx-tools/0x00.py/blob/master/3-print_number.py)
- The output of the script should be:
  - the number, followed by `Battery street`,
  - followed by a new line
- You are not allowed to cast the variable `number` into a string
- Your code must be 3 lines long
- You have to use f-strings [tips](https://realpython.com/python-f-strings/)

```sh
guillaume@ubuntu:~/py/0x00$ ./3-print_number.py
98 Battery street
guillaume@ubuntu:~/py/0x00$ 
```

**Repo**:

- GitHub repository: `alx-higher_level_programming`
- Directory: `0x00-python-hello_world`
- File: `3-print_number.py`

### 4. Print float

Complete this [source code](https://github.com/alx-tools/0x00.py/blob/master/4-print_float.py) in order to print the float stored in the variable `number` with a precision of 2 digits.

- You can find the source code [here](https://github.com/alx-tools/0x00.py/blob/master/4-print_float.py)
- The output of the program should be:
  - `Float:`, followed by the float with only 2 digits
  - followed by a new line
- You are not allowed to cast `number` to string
- You have to use f-strings [tips](https://realpython.com/python-f-strings/)

```sh
guillaume@ubuntu:~/py/0x00$ ./4-print_float.py
Float: 3.14
guillaume@ubuntu:~/py/0x00$ 
```

**Repo**:

- GitHub repository: `alx-higher_level_programming`
- Directory: `0x00-python-hello_world`
- File: `4-print_float.py`

### 5. Print string

Complete this [source code](https://github.com/alx-tools/0x00.py/blob/master/5-print_string.py) in order to print 3 times a string stored in the variable `str`, followed by its first 9 characters.

- You can find the source code [here](https://github.com/alx-tools/0x00.py/blob/master/5-print_string.py)
- The output of the program should be:
  - 3 times the value of `str`
  - followed by a new line
  - followed by the 9 first characters of `str`
  - followed by a new line
- You are not allowed to use any loops or conditional statements
- Your program should be maximum 5 lines long

```sh
guillaume@ubuntu:~/py/0x00$ ./5-print_string.py
HolbertonHolbertonHolberton
Holberton
guillaume@ubuntu:~/py/0x00$
```

**Repo**:

- GitHub repository: `alx-higher_level_programming`
- Directory: `0x00-python-hello_world`
- File: `5-print_string.py`

### 6. Play with strings

Complete this [source code](https://github.com/alx-tools/0x00.py/blob/master/6-concat.py) to print `Welcome to Holberton School!`

- You are not allowed to use any loops or conditional statements.
- You have to use the variables `str1` and `str2` in your new line of code.
- Your program should be exactly 5 lines long.

```sh
guillaume@ubuntu:~/py/0x00$ ./6-concat.py
Welcome to Holberton School!
guillaume@ubuntu:~/py/0x00$
```

**Repo**:

- GitHub repository: `alx-higher_level_programming`

- Directory: `0x00-python-hello_world`
- File: `6-concat.py`

### 7. Copy - Cut - Paste

Complete this [source code](https://github.com/alx-tools/0x00.py/blob/master/7-edges.py)

- You are not allowed to use any loops or conditional statements
- Your program should be exactly 8 lines long
- `word_first_3` should contain the first 3 letters of the variable `word`
- `word_last_2` should contain the last 2 letters of the variable `word`
- `middle_word` should contain the value of the variable `word` without the first and last letters

```sh
guillaume@ubuntu:~/py/0x00$ ./7-edges.py
First 3 letters: Hol
Last 2 letters: on
Middle word: olberto
guillaume@ubuntu:~/py/0x00$
```

**Repo**:

- GitHub repository: `alx-higher_level_programming`
- Directory: `0x00-python-hello_world`
- File: `7-edges.py`

### 8. Create a new sentence

Complete this [source code](https://github.com/alx-tools/0x00.py/blob/master/8-concat_edges.py) to print `object-oriented programming with Python`, followed by a new line.

- You are not allowed to use any loops or conditional statements
- Your program should be exactly 5 lines long
- You are not allowed to create new variables
- You are not allowed to use string literals

```sh
guillaume@ubuntu:~/py/0x00$ ./8-concat_edges.py
object-oriented programming with Python
guillaume@ubuntu:~/py/0x00$
```

**Repo**:

- GitHub repository: `alx-higher_level_programming`
- Directory: `0x00-python-hello_world`
- File: `8-concat_edges.py`

### 9. Easter Egg

Write a Python script that prints “The Zen of Python”, by Tim Peters, followed by a new line.

- Your script should be maximum 98 characters long (please check with `wc -m 9-easter_egg.py`)

```sh
guillaume@ubuntu:~/py/0x00$ ./9-easter_egg.py
The Zen of Python, by Tim Peters

Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
Flat is better than nested.
Sparse is better than dense.
Readability counts.
Special cases aren't special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one-- and preferably only one --obvious way to do it.
Although that way may not be obvious at first unless you're Dutch.
Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it's a bad idea.
If the implementation is easy to explain, it may be a good idea.
Namespaces are one honking great idea -- let's do more of those!
guillaume@ubuntu:~/py/0x00$
```

**Repo**:

- GitHub repository: `alx-higher_level_programming`
- Directory: `0x00-python-hello_world`
- File: `9-easter_egg.py`

### 10. Linked list cycle

Technical interview preparation:

- You are not allowed to google anything
- Whiteboard first

This task is an algorithm challenge. Write a function in C that checks if a singly linked list has a cycle in it.

- Prototype: `int check_cycle(listint_t *list);`
- Return: `0` if there is no cycle, `1` if there is a cycle

Requirements:

- Only these functions are allowed: `write`, `printf`, `putchar`, `puts`, `malloc`, `free`

```sh
carrie@ubuntu:~/0x00$ cat lists.h
#ifndef LISTS_H
#define LISTS_H

#include <stdlib.h>

/**
 * struct listint_s - singly linked list
 * @n: integer
 * @next: points to the next node
 *
 * Description: singly linked list node structure
 * for Holberton project
 */
typedef struct listint_s
{
  int n;
  struct listint_s *next;
} listint_t;

size_t print_listint(const listint_t *h);
listint_t *add_nodeint(listint_t **head, const int n);
void free_listint(listint_t *head);
int check_cycle(listint_t *list);

#endif /* LISTS_H */
carrie@ubuntu:~/0x00$ cat 10-check_cycle.c
#include <stdlib.h>
#include "lists.h"

/**
 * check_cycle - checks if a singly linked list has a cycle in it
 * @list: pointer to the list
 *
 * Return: 0 if there is no cycle, 1 if there is a cycle
 */
int check_cycle(listint_t *list)
{
  listint_t *slow = list;
  listint_t *fast = list;

  while (slow && fast && fast->next)
  {
    slow = slow->next;
    fast = fast->next->next;
    if (slow == fast)
      return (1);
  }

  return (0);
}
carrie@ubuntu:~/0x00$
```

**Repo**:

- GitHub repository: `alx-higher_level_programming`
- Directory: `0x00-python-hello_world`
- File: `10-check_cycle.c`, `lists.h`

### 11. Hello, write

Write a Python script that prints exactly `and that piece of art is useful - Dora Korpar, 2015-10-19`, followed by a new line.

- Use the function `write` from the `sys` module
- You are not allowed to use `print`
- Your script should print to `stderr`
- Your script should exit with the status code `1`

```sh
guillaume@ubuntu:~/py/0x00$ ./100-write.py
and that piece of art is useful - Dora Korpar, 2015-10-19
guillaume@ubuntu:~/py/0x00$ echo $?
1
guillaume@ubuntu:~/py/0x00$
```

**Repo**:

- GitHub repository: `alx-higher_level_programming`
- Directory: `0x00-python-hello_world`
- File: `100-write.py`

### 12. Compile

Write a script that compiles a Python script file.

The Python file name will be stored in the environment variable `$PYFILE`

The output filename has to be `$PYFILEc` (ex: `export PYFILE=my_main.py` => output filename: `my_main.pyc`)

```sh
guillaume@ubuntu:~/py/0x00$ cat main.py
#!/usr/bin/python3
print("Best School")
guillaume@ubuntu:~/py/0x00$ export PYFILE=main.py
guillaume@ubuntu:~/py/0x00$ ./101-compile
Compiling main.py ...
guillaume@ubuntu:~/py/0x00$ ls
101-compile  main.py  main.pyc
guillaume@ubuntu:~/py/0x00$ file main.pyc
main.pyc: compiled Python script, version 3.8
guillaume@ubuntu:~/py/0x00$
```

**Repo**:

- GitHub repository: `alx-higher_level_programming`
- Directory: `0x00-python-hello_world`
- File: `101-compile`

### 13. ByteCode -> Python #1

Write the Python function `def magic_calculation(a, b):` that does exactly the same as the following Python bytecode:

```sh
  3           0 LOAD_CONST               1 (98)
        2 LOAD_FAST                0 (a)
        4 LOAD_FAST                1 (b)
        6 BINARY_POWER
        8 BINARY_ADD
       10 RETURN_VALUE
```

**Repo**:

- GitHub repository: `alx-higher_level_programming`
- Directory: `0x00-python-hello_world`
- File: `102-magic_calculation.py`
