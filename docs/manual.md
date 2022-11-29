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

Now that you've (hopefully) followed one of the installation guides, we can cover how to use Linux's command-line interface (CLI). For most programmers, this is the primary reason they use Linux. If you are using a linux server or a development container, you should already have access to the CLI directly. However, if you are running Linux off of a flashdrive or are using a virutal machine you may have to locate the terminal/command-line application.

Typically, a command is composed of three elements separated by one or more spaces: a name, a list of options, and a list of arguments. 

### Name
The name of a command always comes first. Technically, it is the name of the program we are trying to run. This may seem strange intitially, but every basic function of an operating system, when it comes down to it, is just a program. When you run a program from CLI, it searches for it in dedicated directories (usually /usr/bin/). Once the program is located, it may then be loaded from its file. 

### Options
The options of a command are parameters used to change the program's behavior. They are preceded by either a dash or a double dash.

### Arguments
The arguments of a command are the actual values the program uses as input, such as a number, a file, or a text input. 

---

## Commonly Used Commands

---

### [ls]

list directory contents

Usage:

> ls [OPTION]... [FILE]...

Options:
* **-a, --all**: do not ignore entries starting with ".". This allows you to find hidden files. Generally, software developers will hide important files or backups by prefixing "." to the file name, making them normally invisible to the user.
*

Examples:

```

```
---

### pwd

### [touch]

Update the timestamp of a file, or create a an empty file that does not yet exist.

Usage:

> touch [OPTION]... FILE...


Examples:

```

```
---

### [man]

An interface to the system reference manuals.

Usage:

> man [man options] [[section] page ...] ...

Examples:

```

```

---

### [cd]

Change the working directory.

Usage:

> cd [-L|-P] [directory]

Examples:

```

```

---

### [mkdir]

Make a directory/folder

Usage:

> mkdir [OPTION]... DIRECTORY...

Examples:

```

```

### [rm]

Removes a file or a directory

Usage:

> rm [OPTION]... [FILE]...

Options:
* **-r, -R, --recursive** 
* **-f, --force**

Examples:

```

```
---

### [cp]

copies files or directories

Usage:

> cp [OPTION]... SOURCE DEST
> cp [OPTION]... SOURCE... DIRECTORY

Options:
* **-n, --no-clobber** 
* **-u, --update**
* **-R, -r, --recursive**

Examples:

```

```
---

### [mv]

Move or rename a file

Usage:

> mv [OPTION]... SOURCE DEST
> mv [OPTION]... SOURCE... DIRECTORY

Options:
* **-n, --no-clobber** 
* **-u, --update**

Examples:

```

```

---

## Other Helpful Tools

### apt-get

### vim

### zip


---

## More Complete Documentation


[ls]: https://man7.org/linux/man-pages/man1/ls.1.html
[touch]: https://man7.org/linux/man-pages/man1/touch.1.html
[man]: https://man7.org/linux/man-pages/man1/man.1.html
[cd]: https://man7.org/linux/man-pages/man1/cd.1p.html
[mkdir]: https://man7.org/linux/man-pages/man1/mkdir.1.html
[rm]: https://man7.org/linux/man-pages/man1/rm.1.html
[cp]: https://man7.org/linux/man-pages/man1/cp.1.html
[mv]: https://man7.org/linux/man-pages/man1/mv.1.html