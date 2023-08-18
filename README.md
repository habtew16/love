# Simple Shell Project

A simple shell project developed in C that provides basic shell functionalities.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- - [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Compilation](#compilation)
  - [Usage](#usage)
- [Commands](#commands)
- [Built-in Functions](#built-in-functions)
- [File Structure](#file-structure)
- [Author](#author)
- [License](#license)

## Introduction

The Simple Shell Project is a command-line interpreter implemented in C, providing users with a basic shell environment to execute commands and interact with their system. It is developed as part of a learning exercise to understand shell concepts and C programming.

## Features

- Execute commands from the system's PATH.
- Handle built-in commands like `exit` and `env`.
- Provide basic error handling and user-friendly feedback.
- Supports environment variables and command-line arguments.

## Getting Started

### Prerequisites

Before compiling and running the shell, ensure you have the following:

- A C compiler (e.g., GCC)
- A POSIX-compatible operating system (Linux, macOS)

### Compilation

To compile the shell, use the following command:

```bash
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh
