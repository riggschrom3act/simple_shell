Simple Shell

A lightweight UNIX-style command interpreter written in C.
Originally developed as part of the Holberton School curriculum and migrated here for continued development and portfolio demonstration.

This version implements a basic shell loop capable of reading commands, executing them, and exiting gracefully. Over the next week, the project will progress toward a more complete shell implementation.

 Current Features

Interactive prompt: ($)

Executes commands through system()

Handles user input with buffer & newline trimming

Detects interactive vs non-interactive mode

Graceful exit on:

exit

Ctrl+D (EOF)

Displays a custom error for unknown commands

Persistent loop until exit requested

This is a Stage 1 shell: it runs commands, loops, exits properly, and handles input cleanly.

 Example

Start the shell:

./simple_shell


Run commands:

ls
pwd
echo "Hello"


Exit:

exit


Or press Ctrl+D.

 Current Limitations

This is an intentionally minimal shell for learning and demonstration:

Feature	Status
system() used for execution	 Currently implemented
fork/execve/wait execution	 Not yet
PATH searching	 Not yet
Built-ins beyond exit	 Not yet
Semicolon command chaining	 Not yet
Redirection & pipes	 Not yet
Memory management w/ free()	In progress later
Advanced error formatting- Upcoming
Roadmap (Next Week Development Plan)

The following features will be implemented in phases (commits will reflect each milestone):

Milestone	Target Feature
 Phase 1	Replace system() with fork(), execve(), wait()
 Phase 2	PATH handling
 Phase 3	Basic built-ins (exit, env, cd)
 Phase 4	Semicolon-separated commands
 Phase 5	Error formatting identical to /bin/sh
 Phase 6	Memory management / free() discipline
 Phase 7	Optional: redirection & pipes

Progress logging will appear in commit messages & README updates.

Compilation
gcc -Wall -Werror -Wextra -pedantic *.c -o simple_shell

Usage
./simple_shell


Prompt appears:

($)


Enter commands, or type exit.

File Structure (current)
simple_shell/
├── README.md
├── man_1_simple_shell
└── simple_shell.c    (coming soon)

Authors

Joshua Riggs
Ashly Riggs

Notes

This project began as an academic exercise and is now being actively developed and improved as part of a professional engineering portfolio. Future commits will demonstrate incremental system-level improvements and shell behavior enhancements.

Want to Help?

Educational project — contributions and suggestions welcome.
Please open an issue or pull request.

Status

Current stage: Basic interactive mini-shell
Development style: Incremental upgrades + commit logs over time