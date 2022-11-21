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