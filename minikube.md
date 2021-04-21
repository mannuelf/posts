---
title: "Minikube"
excerpt: "Minikube is a tool which allows you to run a single node Lubernetest cluster on your computer."
coverImage: "/assets/blog/dynamic-routing/cover.jpg"
date: "2020-03-16T05:35:07.322Z"
author:
  name: "M Ferreira"
  picture: "https://res.cloudinary.com/mannuel/image/upload/v1604067445/images/mee.jpg"
ogImage:
url: "https://res.cloudinary.com/mannuel/image/upload/v1604067445/images/mee.jpg"
---

# Minikube, Docker &amp; Kubernetes

If you want to a Kubernetes cluster on you computer, you have 3 options, [Kind](https://kind.sigs.k8s.io/docs/), [kubeadm](https://kubernetes.io/docs/reference/setup-tools/kubeadm/) and [minikube](https://minikube.sigs.k8s.io/docs/).

I will focus on minikube. It supports the latest Kubernetes release, is cross-platform you can use on Linux, macOS or Windows. You can deploy it as VM (Virtual Machine), a container or on bare-metal. minikube supports multiple container runtimes not just Docker, you can use CRI-O, containerd.

## Why would I need this?

If you would like to run a local version of your applications multi container architecture on your local development environment this is a way to do it.

## Installation

I will focus on macOS. Other installation instructions available ([Linux](https://minikube.sigs.k8s.io/docs/start/), [Windows](https://minikube.sigs.k8s.io/docs/start/))

```bash
brew install minikube
```

### Start cluster

Check the help documentation, and confirm installation was successfull.

```bash
minikube
```

[001]

Start minikube cluster.

```bash
minikube start
```

[002]

At this point you can confirm things by running, status and testing to see if kubectl is also instsalled as part of the minukube installation process.

```bash
minikube status
```

Check current running pods. minikube has a few pods already you can check this by running the `kubectl` command passing the 'all' flag `-A`.

```bash
kubectl get po -A
```

[003]

In this output you can see the:

- namespace
- name
- ready state
- status,
- restart state
- age

Later we will configure a new project namespace to differniate our projects from kube-system pods.
