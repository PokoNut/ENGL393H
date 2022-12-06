---
layout: default
title: History of Linux
nav_order: 3
---

# History of Linux
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## The Unix Operating System

The Unix operating system was originally created in the late 1960s, developed at Bell Labs by a group of AT&T employees. While it was intended for use solely inside Bell Labs, AT&T licensed Unix for outside use in the late 1970s. 

Unix is characterized by a number of features made distinct from other operating systems:

### Portability

Simply put, the definition of software portability is the level of difficulty required to make a given piece of software run on any platform. An operating system with high portability should run on any kind of hardware, but one with low portability would be confined. It may seem like Windows and MacOS are already portable enough, but this is often only the case in personal computing. Unix pioneered the ability to run on many platforms, making it popular in industry.

### Multitasking

Modern operating systems can have many different applications running at the same time. This is referred to as multitasking, or the ability to divide the processor's time between many tasks. Technically, it only looks like everything is running at the same time (although modern processors actually can run multiple processes). Unix was the first operating system to implement such a concept.

### Hierarchical File System

The file system is how drives and files are organized in an operating system. The principal unit of storage is called a "directory", which is analogous to a folder. Directories can store files or other directories. This makes file management and browsing much more convenient for users. 


Despite its age, Unix is still a very modern, portable, and multitasking operating system. 

---

## Why was Linux Made?

Since Unix is so effective, why isn't it more popular? The answer can be found in the "Unix wars", a series of disputes over copyright between software companies. Because of its popularity, many software companies sought to monopolize Unix and create their own closed ecosystem to trap users (sound familiar?). In this pursuit, however, many competitors neglected to focus on the actual product. Most Unix clones were incomplete and unstable.

Enter Richard Stallman, the creator of the Free Software Foundation and an MIT labs programmer. Throughout his career, he saw for himself the dangers that closed software posed to users. He believed that the user should be free to create, study, use, modify, and essentially do whatever they wanted with their software[[1]]. It should be noted that free software should not necessarily be given away, but it should not be artificially limiting the user. 

To avoid predatory copyright use, Richard came up with the idea of "copyleft". Copyleft is a special kind of copyright, with its only limitation being that any work registered under copyleft must not prevent sharing. Additionally, every modification or addition to software under copyleft **must** be licensed under similar rules. Thus, the concept of open source was born.

---

## The Linux Kernel and GNU

In 1991, a university student named Linus Torvalds purchsed an Intel IBM PC. He was disappointed with the operating systems available for his computer, so he started creating a terminal emulator based on Minix, another Unix-like operating system[[1]].

Torvalds wanted his operating system to do more things, but he did not have the resources available to do so. It was then that he posted a message to Minix user group, saying "I'm doing a (free) operating system (just a hobby, won't be bing and professional like gnu) for 386(486) AT clones." What followed is now called the most important collaborative effort in the history of computers[[1]]. 

Despite the efforts of Linus and many of his collaborators, Linux was not a complete operating system. It had no applications or programs to run on top of it, so it was fairly useless on its own. Fortunately, a separate project consisting of a collection of free tools and applications called GNU (piloted by Richard Stallman) was searching for an open-source, Unix-like kernel. So, GNU was integrated into Linux and GNU/Linux was born.

It is technically most accurate to call Linux GNU/Linux, but many  programmers simply refer to the project as Linux. For simplicity, I will continue to use Linux. 

---

[[1]]: Raggi, E. (2011). Beginning ubuntu linux (6th ed., Ser. The expert's voice in linux). Apress. https://doi.org/10.1007/978-1-4302-3627-6 

