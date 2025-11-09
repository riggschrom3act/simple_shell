# Simple Shell

A lightweight Unix-style command interpreter written in C.  
Originally developed as part of the Holberton School low-level programming curriculum and later migrated to this profile for portfolio archiving and ongoing improvements.

This project demonstrates core systems programming concepts including process creation, command parsing, memory management, and environment handling.

---

## Features

- Execute basic shell commands  
- Handle command paths & built-ins  
- Read and interpret user input  
- Support for semicolon command chaining  
- Error handling & exit status behavior  
- Shell loop using `fork/exec/wait` and low-level read/write syscalls

---

## Installation

```bash
# Clone the repo
git clone https://github.com/<your-username>/simple_shell.git
cd simple_shell

# Compile
gcc -Wall -Werror -Wextra -pedantic *.c -o simple_shell

# Run
./simple_shell
 Usage

Start the shell:

./simple_shell


Then enter commands like:

ls
pwd
echo "Hello, world"


Keyboard shortcuts:

↑ / ↓ – command history (limited)

CTRL-D – exit

CTRL-C – interrupt current command

Project Scope & Limitations

This shell was created as a learning exercise.
It does not currently support:

Pipes (|), redirection (>, <<), or background &

Aliases

Job control

Full environment variable expansion

This behavior mirrors early Bourne-like shells and is intended to demonstrate foundational systems concepts.

Future improvements may include:

Pipe chaining

File redirection support

Built-in command expansion

Extended environment manipulation

Contributing

This is an educational project, but suggestions and improvements are welcome.

To contribute:

fork → branch → commit → pull request


Issues may be opened for bugs, code improvements, or feature suggestions.

Authors

Joshua Riggs — Developer
Ashly Riggs — Collaborator
Holberton School Software Engineering Program

Footnote

Migrated from academic repo for portfolio completeness and to demonstrate version control beyond school environment. Continuing incremental improvements and documentation updates.
