---
title: 'Docker one o one'
excerpt: 'Docker allows developers to build software in a container environment. Instead of Virtual Machines which are cumbersome Docker is light weight and allows you to isolate your program and development to a single container.'
coverImage: '/assets/blog/dynamic-routing/cover.jpg'
date: '2021-02-09T22:10:35+00:00'
author:
  name: M Ferreira
  picture: 'https://res.cloudinary.com/mannuel/image/upload/v1604067445/images/mee.jpg'
ogImage:
  url: 'https://res.cloudinary.com/mannuel/image/upload/v1604067445/images/mee.jpg'
---

## What is Docker

> A standardized unit of software"

- docker.com

Docker is container runtime environment. It isolates all dependencies required to build and run an application into one neat and small (mostly) container.

### So what?

Well instead of installing Node.js, NPM, NVM, MongoDB, PHP on your LAPTOP all you have to do is pull down a Docker IMAGE that already has that software packaged inside of it. All you have to do use it, build you code in it.

![node](./.images/node-image.png)

```bash
docker pull node
```

You manage your containers using the Docker application on your development machine.

You manage your containers using the docker CLI (command line interface)

You can

- create
- delete
- publish
- configure

## Install Docker

![install](.images/docker-desktop.png)

## Clone image

```bash
docker run --name repo alpine/git clone https://github.com/docker/getting-started.git
```

```bash
docker cp repo:/git/getting-started/ .
```

## Build container

```bash
docker build -t docker101tutorial .
```

## Run your first container

```bash
docker run -d -p 80:80 --name docker-tutorial docker101tutorial
```

## Now save and share your image

Save and share your image on Docker Hub to enable other users to easily download and run the image on any destination machine.
