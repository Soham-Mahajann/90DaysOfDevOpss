# 🚀 Day 02 - Linux Architecture, Processes & systemd

# 🐧 1️⃣ Core Components of Linux

Linux is a operationg system which is made up of three major components which work together to run the operating system.
Everything in linux is either a file, folder, or a process.

The Architecture of Linux is based on "ASK" structure

- A - Application
- K - Kernal
- S - Shell

## 🔹 Application 

- The **Application** can be any software which is used by the user for executing the required operation. 
- eg - Terminal, notepad, gedit etc

## 🔹 Shell 

- These are mmostly the commands which are used in linux.
- Shell works as  the interface between application and kernal.

## 🔹 Kernel

- The **Kernel** is the heart of the Linux operating system.
- Linus kernal is written in "C" language.

### Responsibilities:
- Manages the CPU
- Manages Memory (RAM)
- Controls Storage Devices
- Manages Hardware Devices
- Handles communication between hardware and applications using **System Calls**

Without the kernel, Linux cannot function.

---

## 🔹 User Space

User Space is where users interact with the operating system.

It includes:

- Bash Shell
- Terminal
- System Utilities
- Installed Applications
- User Programs

Applications running in User Space cannot directly access the hardware. They communicate with the Kernel through **System Calls**.

# ⚙️ 2️⃣ How Processes Are Created & Managed

A **Process** is a running instance of a program.

Every process in Linux has a unique **Process ID (PID)**.

### Process Creation

Linux creates processes using two important system calls:

### 🔹 fork()

- Creates a new child process.
- The child process is almost identical to the parent process.

### 🔹 exec()

- Replaces the current process with a new program.
- Used after `fork()` to execute another application.

# 🔄 3️⃣ Process States

A process can exist in different states during its lifecycle.

| State | Meaning |
|--------|---------|
| **R (Running)** | Process is currently executing on the CPU. |
| **S (Sleeping)** | Waiting for user input or another resource. |
| **T (Stopped)** | Process has been paused or suspended manually. |
| **Z (Zombie)** | Process has finished execution, but its parent hasn't collected its exit status. |
| **D (Uninterruptible Sleep)** | Waiting for disk or I/O operations to complete. |

Understanding process states helps troubleshoot:

# 💻 4️⃣ Daily Linux Commands

-  pwd - Print the current working directory.
- Is - List files and directories.
- cd - Change directory.
- cd / - root directory.
- cd ~ - one step back.
- ping - check internet.
- touch - Create an empty file.
- mkdir - Create a new directory.
- vim - it is a editor (i = insert ; esc ; :wq = to exit)
- rm - Remove files or directories.
- rmdir - Remove empty directories.
- cp - Copy files or directories.
- mv - Move or rename files and directories.
- cat - Display the content of a file.
- echo - Display a line of text.
- clear - Clear the terminal screen.

