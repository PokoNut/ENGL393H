---
layout: default
title: VSCode Dev Container
parent: Developing in a Linux Environment
nav_order: 2
---

# VSCode Development Container
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## What is a Container?

A container is essentailly an entire runtime environment: an application, its dependencies, and libraries. They are a form of operating system virtualization. It can be helpful to conceptualize them as miniature virtual machines, with much of the functionality stripped away.

Usually, these are used to package software so that it may run reliablely on any computer. However, we may repurpose them as a full-featured development environment with all of the usual Linux command-line tools. 

## Requirements

You will need to install [docker] desktop and [visual studio code] respectively. 

## Steps

### Install VSCode Docker Extensions

![](../../assets/container1.png)

### Open Folder in Remote in Container

![](../../assets/container2.png)
![](../../assets/container3.png)

[docker]: https://www.docker.com/products/docker-desktop/
[visual studio code]: https://code.visualstudio.com/ 
[VSCode]: https://code.visualstudio.com/docs/devcontainers/containers
[Docker]: https://docs.docker.com/desktop/dev-environments/create-dev-env/

