# Docker Basics and Usage

This repository documents my learning journey with Docker. It includes explanations, examples, and best practices for using Docker effectively.

---

## Table of Contents
1. [What is Docker?](#what-is-docker)
2. [Why Use Docker?](#why-use-docker)
3. [Docker vs. Virtual Machines](#docker-vs-virtual-machines)
4. [Docker Commands and CLI](#docker-commands-and-cli)
5. [Creating a Dockerfile](#creating-a-dockerfile)
6. [Building and Pulling Docker Images](#building-and-pulling-docker-images)
7. [Port Binding and Networking](#port-binding-and-networking)
8. [Using Docker Desktop](#using-docker-desktop)
9. [Resources](#resources)

---

## What is Docker?
Docker is a platform for developing, shipping, and running applications in isolated environments called containers. It solves problems like:
- Inconsistent environments across development, testing, and production.
- Large overhead of virtual machines compared to lightweight containers.

---

## Why Use Docker?
- **Consistency**: Applications run the same across different environments.
- **Efficiency**: Lightweight and fast compared to VMs.
- **Isolation**: Prevents conflicts between dependencies.
- **Portability**: Runs anywhere with Docker installed.

---

## Docker vs. Virtual Machines
| **Aspect**        | **Docker (Containers)** | **Virtual Machines** |
|--------------------|-------------------------|-----------------------|
| Isolation          | Process-level          | Hardware-level        |
| Size               | Lightweight (MBs)      | Heavy (GBs)           |
| Startup Time       | Seconds                | Minutes               |
| Performance        | Near-native            | Moderate              |
| Resource Usage     | Shared OS kernel       | Full OS instance      |

---

## Docker Commands and CLI
### Common Commands:
- `docker run`: Run a container.
- `docker build`: Build an image from a Dockerfile.
- `docker pull`: Pull an image from Docker Hub.
- `docker ps`: List running containers.
- `docker stop`: Stop a running container.
- `docker rm`: Remove a container.
- `docker images`: List available images.
- `docker rmi`: Remove an image.

[Full list of commands](https://docs.docker.com/engine/reference/commandline/docker/)

---

## Creating a Dockerfile
- Use the official Apache HTTP Server image
   -- FROM httpd:2.4

- Copy static website files to the Apache server's web root
   -- COPY ./public-html/ /usr/local/apache2/htdocs/
---
