# Linux Introduction

## What is Linux?

Linux is a free and open-source, Unix-like operating system based on the Linux kernel.

It is widely used in:

- Servers
- Cloud platforms
- Containers
- Smartphones
- Embedded devices
- DevOps environments

Linux is important for DevOps because most cloud servers, containers, CI/CD tools, and Kubernetes nodes run on Linux.

## Linux Artchitecture 

<img width="882" height="501" alt="image" src="https://github.com/user-attachments/assets/e4b4109a-40ab-4763-9220-f21a67510ece" />

Linux can be understood using the following layers:

```text
User
  ↓
Application
  ↓
Shell
  ↓
Kernel
  ↓
Hardware
```

## Components of Linux

### 1. Hardware

Physical components of the computer, such as:

- CPU
- RAM
- Disk
- Network interface

### 2. Kernel

The kernel is the core of the operating system.

It manages:

- CPU
- Memory
- Devices
- Processes
- System resources

The kernel provides communication between software and hardware.

### 3. Shell

The shell is an interface between the user and the operating system.

Examples:

- Bash
- Zsh
- Sh

It accepts commands and sends them to the operating system for execution.

### 4. Applications

Applications are programs that run on Linux.

Examples:

- Nginx
- Docker
- Git
- Jenkins
- Python

### 5. User

The user interacts with Linux through either the command line or graphical interface.

## CLI vs GUI

### CLI

CLI stands for Command-Line Interface.

Advantages:

- Faster for experienced users
- Requires fewer system resources
- Suitable for automation
- Commonly used on servers
- Useful for shell scripting

Examples:

```bash
ls
pwd
mkdir project
```

### GUI

GUI stands for Graphical User Interface.

Advantages:

- Easier for beginners
- Uses icons, menus, and windows
- Does not require memorising commands

However, GUI usually consumes more resources and is less suitable for server automation.

## Why DevOps Engineers Use Linux

DevOps engineers use Linux for:

- Managing cloud servers
- Running containers
- Creating shell scripts
- Automating deployments
- Troubleshooting applications
- Managing files, users, and services
