# Command Line Basics


## Table of Contents

  - [Lecture 2: Command Line Basics](#lecture-2-command-line-basics)
    - [The Command Line Interface (CLI)](#the-command-line-interface-cli)
    - [Common Commands in Operating Systems](#common-commands-in-operating-systems)
      - [The `echo` Command](#the-echo-command)
      - [Displaying Date and Time Manipulation](#displaying-date-and-time-manipulation)
    - [Navigating Directories](#navigating-directories)
      - [Directory Structures](#directory-structures)
      - [Navigation Commands](#navigation-commands)
    - [File and Directory Management](#file-and-directory-management)
    - [Manipulating Files](#manipulating-files)
    - [Searching and Patterns](#searching-and-patterns)
    - [Shortcuts and Aliases](#shortcuts-and-aliases)
    - [Conclusion](#conclusion)
   
## The Command Line Interface (CLI)

- The Command Line Interface, or CLI, is a textual interface to interact with a computer. Instead of using graphical elements like buttons or menus, users type commands into a prompt.
- CLI is often used for tasks that require precise control, automation, or when managing remote machines.

## Common Commands in Operating Systems

### The `echo` Command

- The `echo` command is utilized to print text or data to the console. It's a foundational command used in various operating systems, scripting languages, and programming contexts.
  
  **Example:**
  ```bash
  # Printing a simple message
  echo "Hello, World!"
  ```
  ```
  Hello, World!
  ```

  ```bash
  # Displaying the current date and time
  echo $(date)
  ```

### Displaying Date and Time Manipulation

- **`date` Command**: This command displays the current date and time, but can also be used to display a future or past date by using the `-d` option and providing a specific string, like "next Monday".

  ```bash
  # Display the current date and time
  date
  ```

  ```bash
  # Display the date and time of the next Monday
  date -d "next Monday"
  ```

- **Custom Formatting**: The `date` command can also be combined with a custom formatting string to display specific parts of the date or rearrange its presentation.

  ```bash
  # Display a message with a custom formatted date
  date -d "next Monday" + "The deadline is at %d.%m.%Y %H:%M:%S Uhr"
  ```

  In this example:
  - `%d` is the day of the month.
  - `%m` is the month.
  - `%Y` represents the year.
  - `%H`, `%M`, and `%S` are hours, minutes, and seconds respectively.
  - "Uhr" is German for "hour" or "clock", indicating the time.
 
## Navigating Directories

### Directory Structures

- In different operating systems, the method to refer to directories varies.

  - **Windows**: Uses drive letters like `C:/` or `D:/`.
  - **Linux**: Uses a hierarchical structure starting from the root directory, denoted as `/`.

### Navigation Commands

- **`pwd`**: Short for 'print working directory', this command displays the directory you're currently in.
  
  **Example:**
  ```bash
  # Displaying the current directory
  pwd
  ```

- **`cd`**: Used to navigate between directories. Short for 'change directory'.
  
  ```bash
  # Navigating to a specific directory
  cd /home/user/Documents
  ```

  ```bash
  # Navigating to the parent directory
  cd ../
  ```

- **`ls`**: Lists files and directories in the current location.
  
  ```bash
  # Listing files in the current directory
  ls
  ```

  ```bash
  # Detailed list of files in the 'Downloads' directory
  ls -l Downloads
  ```

## File and Directory Management

- **`mkdir`**: This command creates a new directory.
  
  ```bash
  # Creating a new directory named 'new_folder'
  mkdir new_folder
  ```

- **`cat`**: Displays the contents of a file.
  
  ```bash
  # Displaying the contents of a file named 'filename.txt'
  cat filename.txt
  ```

- **`rm`**: This command is used to remove objects such as files, directories, and symbolic links from the filesystem. By default, it does not remove directories.

  ```bash
  # Removing a file
  rm filename.txt
  ```

  ```bash
  # Recursively removing a directory and its contents
  rm -r directory_name
  ```

### Manipulating Files

- **`cp`**: Stands for 'copy'. It's used to duplicate files or directories.
  
  ```bash
  # Copying 'source.txt' to 'destination.txt'
  cp source.txt destination.txt
  ```

  ```bash
  # Copying 'file.txt' into the 'folder' directory
  cp file.txt folder/
  ```

- **`mv`**: Short for 'move'. It can move files between directories or rename them.
  
  ```bash
  # Moving 'source.txt' into 'folder' directory
  mv source.txt folder/
  ```

  ```bash
  # Renaming 'oldname.txt' to 'newname.txt'
  mv oldname.txt newname.txt
  ```

### Searching and Patterns

- **`ls` with Patterns**: Using patterns can help filter and list specific files.
  
  ```bash
  # Listing all .txt files in the current directory
  ls *.txt
  ```

  ```bash
  # Listing files with exactly 6 characters before the `.txt` extension
  ls ??????.txt
  ```

## Shortcuts and Aliases

- **`alias`**: This command creates shortcuts for other commands or a series of commands, enhancing efficiency.

  ```bash
  # Creating an alias 'll' to display a detailed list of files
  alias ll="ls -l"
  ```

## Conclusion

Mastering command-line utilities is crucial for efficiently navigating and managing operating systems, especially in environments without a graphical user interface. The commands discussed in this lecture provide a foundational understanding, but many more commands and functionalities can be explored in the vast realm of operating systems.
