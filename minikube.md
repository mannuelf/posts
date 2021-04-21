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

# Minikube

If you want to a Kubernetes cluster on you computer, you have 3 options, [Kind](https://kind.sigs.k8s.io/docs/), [kubeadm](https://kubernetes.io/docs/reference/setup-tools/kubeadm/) and [minikube](https://minikube.sigs.k8s.io/docs/).

I will focus on minikube. It supports the latest Kubernetes release, is cross-platform you can use on Linux, macOS or Windows. You can deploy it as VM (Virtual Machine), a container or on bare-metal. minikube supports multiple container runtimes not just Docker, you can use CRI-O, containerd.
