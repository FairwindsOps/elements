# Fairwinds Elements
Fairwinds Elements is a suite of open source software to help manage Kubernetes infrastructure at enterprise scale backed by support from Fairwinds.

Getting the right in-house expertise and cluster add-ons to get to production-ready Kubernetes in a consistent way across organizations is still out of reach for many. Once in production, adding clusters with consistent configurations is complicated. 

How do you find the right add ons, what are best practices for using them, and how do they all work together cohesively? Fairwinds Elements is a clear and trusted answer to these problems, to increase speed to production and reduce trial-and-error exponentially.

There are other solutions out there that provide opinionated setups and software but require vendor lock-in. Fairwinds Elements leverages best-in-class Open Source tooling in a cohesive way to provide a "vanilla Kubernetes" setup independant on any single vendor.

To **get started** with **Fairwinds Elements** please read the [Quick Start Guide](/quickstart/).

Visit [https://www.fairwinds.com/elements](https://www.fairwinds.com/elements) for more information on why you should use **Fairwinds Elements** or to get in touch about a support subscription.

This repository contains the source code for Fairwinds Elements documentation. If you're looking for individual components, they live in their own repositories.

Please see below for links and descriptions of each component:

### Cluster Add-Ons
- [RBAC-manager](https://github.com/FairwindsOps/rbac-manager) - This is an operator that supports declarative configuration for RBAC with new custom resources. Instead of managing role bindings or service accounts directly, you can specify a desired state and RBAC Manager will make the necessary changes to achieve that state.
- [metrics-server (AWS only)](https://github.com/kubernetes-sigs/metrics-server) - https://github.com/kubernetes-sigs/metrics-server
- [nginx-ingress](https://github.com/kubernetes/ingress-nginx) - Controller to manage Nginx configurations base on Kubernetes Ingress objects
- [cert-manager](https://github.com/jetstack/cert-manager) - Automatically provision and manage TLS certificates in Kubernetes
- [external-dns](https://github.com/kubernetes-sigs/external-dns) - ExternalDNS synchronizes exposed Kubernetes Services and Ingresses with DNS providers.
- [metrics-server](https://github.com/kubernetes-sigs/metrics-server) - Provides resource usage metrics, such as container CPU and memory usage.
- [cluster-autoscaler](https://github.com/kubernetes/autoscaler) - Automatically adjusts the size of a Kubernetes Cluster so that all pods have a place to run and there are no unneeded nodes.
- [aws-alb-ingress-controller](https://github.com/kubernetes-sigs/aws-alb-ingress-controller) - The AWS ALB Ingress Controller satisfies Kubernetes ingress resources by provisioning Application Load Balancers.
- [aws-iam-authenticator](https://github.com/kubernetes-sigs/aws-iam-authenticator) - A tool to use AWS IAM credentials to authenticate to a Kubernetes cluster. 

### Operator Tools
- [RBAC-Lookup](https://github.com/FairwindsOps/rbac-lookup ) - RBAC Lookup is a CLI that allows you to easily find Kubernetes roles and cluster roles bound to any user, service account, or group name. Binaries are generated with goreleaser for each release for simple installation.
- [Astro](https://github.com/FairwindsOps/astro) - Astro is a Kubernetes operator that watches objects in your cluster for defined patterns, and manages DataDog monitors based on this state.
- [rok8s-scripts](https://github.com/FairwindsOps/rok8s-scripts) - rok8s-scripts is a framework for building GitOps workflows with Docker and Kubernetes. By adding rok8s-scripts to your CI/CD pipeline, you can build, push, and deploy your applications using the set of best practices we've built at Fairwinds.
- [Reckoner](https://github.com/FairwindsOps/reckoner) - Reckoner is a command line helper for Helm that uses a YAML syntax to install and manage multiple Helm charts in a single file and allows installation of charts from a git commit/branch/release.
- [Polaris](https://github.com/FairwindsOps/polaris ) - Fairwinds' Polaris keeps your clusters sailing smoothly. It runs a variety of checks to ensure that Kubernetes pods and controllers are configured using best practices, helping you avoid problems in the future. — Polaris is also available in Fairwinds Insights.
- [Goldilocks](https://github.com/FairwindsOps/goldilocks ) - By using the Kubernetes vertical-pod-autoscaler in recommendation mode, we can see a suggestion for resource requests on each of our apps. Goldilocks creates a VPA for each deployment in a namespace and then queries them for information. —
Goldilocks is also available in Fairwinds Insights.
- [Fairwinds Terraform Library](NEEDSLINK) - Fairwinds Terraform Library

We welcome your input. If you have feedback, please [submit an issue][issues]. If you'd like to participate in development, please read the "Working on Documentation" section below and [submit a pull request][prs].

# Working on Documentation

The Elements project welcomes contributions from all developers. The high level process for development matches many other open source projects. See below for an outline.

* Fork this repository.
* Make your changes.
* [Submit a pull request][prs] (PR) to this repository with your changes, and unit tests whenever possible.
	* If your PR fixes any [issues][issues], make sure you write `Fixes #1234` in your PR description (where `#1234` is the number of the issue you're closing).
* The Elements core contributors will review your code. After each of them sign off on your code, they'll label your PR with `LGTM1` and `LGTM2` (respectively). Once that happens, a contributor will merge it.

## Requirements

Fairwinds Elements assumes the existence of Kubernetes, the necessity or value of various components of Fairwinds Elements will change based on where the Kubernetes cluster is running (AWS vs. GCP or Azure vs. Datacenter etc...)

### Local Installation


## Building Documentation



## Serve Documentation Locally

