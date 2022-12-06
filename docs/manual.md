---
layout: default
title: Manual
nav_order: 6
---

# Manual
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Anatomy of a Command

Now that you've (hopefully) followed one of the installation guides, we can cover how to use Linux's command-line interface (CLI). For most programmers, this is the primary reason they use Linux. If you are using a linux server or a development container, you should already have access to the CLI directly. However, if you are running Linux off of a flash drive or are using a virtual machine you may have to locate the terminal/command-line application.

Typically, a command is composed of three elements separated by one or more spaces: a name, a list of options, and a list of arguments. 

### Name
The name of a command always comes first. Technically, it is the name of the program we are trying to run. This may seem strange initially, but every basic function of an operating system, when it comes down to it, is just a program. When you run a program from CLI, it searches for it in dedicated directories (usually /usr/bin/). Once the program is located, it may then be loaded from its file. 

### Options
The options of a command are parameters used to change the program's behavior. They are preceded by either a dash or a double dash. In this guide, I have omitted many less-important options for clarity. Note that you can list arguments separately (-a -b -c ...) or combine them (-abc) for the same effect.

### Arguments
The arguments of a command are the actual values the program uses as input, such as a number, a file, or a text input. When supplying a directory as an argument, you may use "." to refer to the current directory and ".." to refer to the parent directory.

Sometimes, a command may need higher-level permissions to run (similar to how other operating systems may ask for administrator passwords). You can prefix the command with "sudo" to run the command as a "superuser," which is the same as an administrator.

---

## Commonly Used Commands

### [ls]

Lists directory contents. 

Usage:

> ls [OPTION]... [FILE]...

Options:
* **-a, --all**: do not ignore entries starting with ".". This allows you to find hidden files. Generally, software developers will hide important files or backups by prefixing "." to the file name, making them normally invisible to the user.
* **-R, --recursive**: lists subdirectories recursively. In other words, files stored in directories inside the current directory will also be listed.
* **-t**: sorts by time, newest first.

Examples:

```
# List the files in the current directory
ls
file_a  file_b  folder_c


# List all files, including hidden ones
ls -a 
file_a  file_b  folder_c
.file_d  .file_e  .file_f


# List all files, inclding those in folders
ls -R
file_a  file_b  folder_c

./folder_c:
file_d  file_e  file_f
```
---

### [pwd]

Prints the name of the current/working directory.

Usage:

> pwd [OPTION]...

Examples:

```
# Lists the current directory
pwd
/home/bob
```
---


### [touch]

Update the timestamp of a file, or create a an empty file that does not yet exist.

Usage:

> touch [OPTION]... FILE...


Examples:

```
# List files in current directory
ls 
file_a  file_b


# Create a file called file_c
touch file_c


# List files in current directory, there is a new file called file_c
ls
file_a  file_b  file_c
```
---

### [man]

An interface to the system reference manuals. Whenever you are interested in learning how a command works, you can type man and then the name of the command.

Usage:

> man [man options] [[section] page ...] ...

The output for man is too long to list here, but it displays similar information to what you will find from the completed documentation linked on this page. Press q to exit man.

Examples:

```
# Display the manual for ls
man ls


# Display the manual for pwd
man pwd
```

---

### [cd]

Change the working directory.

Usage:

> cd [directory]

Examples:

```
# List files in current directory
ls
folder_a


# Move into the directory folder_a
cd folder_a


# Now that you are in the new directory, you can perform other commands
ls
file_a  file_b  file_c
```

---

### [mkdir]

Make a directory/folder

Usage:

> mkdir [OPTION]... DIRECTORY...

Examples:

```
# Make a directory called folder_a
mkdir folder_a


# Move into the new directory
cd folder_a


# Make a new file inside the directory
touch file_a
```

### [rm]

Removes a file or a directory

Usage:

> rm [OPTION]... [FILE]...

Options:
* **-r, -R, --recursive**: deletes directories and all files in them.
* **-f, --force**: ignore files that do not exist, and never ask for confirmation. 

Examples:

```
# Check contents of directory
ls
file_a  file_b  folder_c


# Remove file_a
rm file_a
remove file? y


# Remove file_b with no confirmation
rm -f file_b


# Remove folder_c with no confirmation
rm -rf folder_c


# Check the directory is now empty
ls

```
---

### [cp]

copies files or directories

Usage:

> cp [OPTION]... SOURCE DEST
> cp [OPTION]... SOURCE... DIRECTORY

Options:
* **-n, --no-clobber**: avoids overwriting an existing file. 
* **-u, --update**: copies only if the SOURCE file is newer than the destination file, or if it is missing.
* **-R, -r, --recursive**: copies recursively. Use this to copy entire folders.

Examples:

```
# List directory contents
ls
file_a  folder_b  folder_c


# Copy file_a into folder_b
cp file_a folder_b

# Copy folder_c into folder_b
cp -r folder_c folder_b


# List directory contents
ls
file_a  folder_b  folder_c
```
---

### [mv]

Move or rename a file

Usage:

> mv [OPTION]... SOURCE DEST
> mv [OPTION]... SOURCE... DIRECTORY

Options:
* **-n, --no-clobber**: moves only if the SOURCE file is newer than the destination file, or if it is missing.
* **-u, --update**: moves recursively. Use this to move entire folders.

Examples:

```
# List directory contents
ls
file_a  folder_b  folder_c  file_d


# Move file_a into folder_b
mov file_a folder_b


# Move folder_c into folder_b
mov -r folder_c folder_b


# Rename file_d into file_z
mov file_d file_z


# List directory contents
ls
folder_c    file_z
```

---

## More Complete Documentation

You can check out further documentation for Linux at the [man-pages] website, an open-source project dedicated to the Linux kernel an GNU libraries.


[ls]: https://man7.org/linux/man-pages/man1/ls.1.html
[touch]: https://man7.org/linux/man-pages/man1/touch.1.html
[man]: https://man7.org/linux/man-pages/man1/man.1.html
[cd]: https://man7.org/linux/man-pages/man1/cd.1p.html
[mkdir]: https://man7.org/linux/man-pages/man1/mkdir.1.html
[rm]: https://man7.org/linux/man-pages/man1/rm.1.html
[cp]: https://man7.org/linux/man-pages/man1/cp.1.html
[mv]: https://man7.org/linux/man-pages/man1/mv.1.html
[pwd]: https://man7.org/linux/man-pages/man1/pwd.1.html
[man-pages]: https://www.kernel.org/doc/man-pages/