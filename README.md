# Fairwinds Elements
Fairwinds Elements is a suite of open source software to help manage Kubernetes infrastructure at enterprise scale used in Fairwinds' ClusterOps Managed Service and/or backed by Fairwinds Elements Support offering.

Getting the right in-house expertise and cluster add-ons to get achieve _and_ operate production-ready Kubernetes in a consistent way across organizations is still out of reach for many. Once in production, adding clusters with consistent configurations is complicated. 

Fairwinds Elements leverages best-in-class Open Source software in a cohesive way to provide a complete platform independant of any single vendor.

Visit [https://www.fairwinds.com/elements](https://www.fairwinds.com/elements) for more information on why you should use **Fairwinds Elements** or to get in touch about a support subscription.

This repository contains the source code for Fairwinds Elements documentation. If you're looking for individual components, they live in their own repositories.

Please see below for links and descriptions of each component:

### Command Line Software
- [RBAC-Lookup](https://github.com/FairwindsOps/rbac-lookup ) - RBAC Lookup is a CLI that allows you to easily find Kubernetes roles and cluster roles bound to any user, service account, or group name. Binaries are generated with goreleaser for each release for simple installation.
- [Reckoner](https://github.com/FairwindsOps/reckoner) - Reckoner is a command line helper for Helm that uses a YAML syntax to install and manage multiple Helm charts in a single file and allows installation of charts from a git commit/branch/release.
- [Pluto](https://github.com/FairwindsOps/pluto) - This is a very simple utility to help users find deprecated Kubernetes apiVersions in their code repositories and their helm releases.
- [Nova](https://github.com/FairwindsOps/Nova) - Nova scans your cluster for installed Helm charts, then cross-checks them against all known Helm repositories. If it finds an updated version of the chart you're using, or notices your current version is deprecated, it will let you know.


## CI/CD Support
- [rok8s-scripts](https://github.com/FairwindsOps/rok8s-scripts) - rok8s-scripts is a framework for building GitOps workflows with Docker and Kubernetes. By adding rok8s-scripts to your CI/CD pipeline, you can build, push, and deploy your applications using the set of best practices we've built at Fairwinds.


### In-Cluster Operations Software
- [Astro](https://github.com/FairwindsOps/astro) - Astro is a Kubernetes operator that watches objects in your cluster for defined patterns, and manages DataDog monitors based on this state.
- [Goldilocks](https://github.com/FairwindsOps/goldilocks ) - By using the Kubernetes vertical-pod-autoscaler in recommendation mode, we can see a suggestion for resource requests on each of our apps. Goldilocks creates a VPA for each deployment in a namespace and then queries them for information. —
Goldilocks is also available in Fairwinds Insights.
- [Gemini](https://github.com/FairwindsOps/gemini) - Gemini is a Kubernetes CRD and operator for managing VolumeSnapshots. This allows you
to back up your PersistentVolumes on a regular schedule, retire old backups, and restore backups with minimal downtime.
- [Polaris](https://github.com/FairwindsOps/polaris ) - Fairwinds' Polaris keeps your clusters sailing smoothly. It runs a variety of checks to ensure that Kubernetes pods and controllers are configured using best practices, helping you avoid problems in the future. — **Polaris is also available in Fairwinds Insights.**


### Cluster Add-Ons

#### Networking & Load Balancing
- **external-dns** - Automate DNS management
- **ingress-nginx** - Manage HTTP and HTTPS routing
- **AWS Load Balancer Controller** - AWS Load Balancer integration
- **AWS VPC CNI** - Native AWS networking for Kubernetes
- **Oauth2 Proxy** - Secure authentication for apps

#### Security & Compliance
- **cert-manager** - Automate TLS certificate management
- **External Secrets** - Securely inject secrets
- **Falco** - Runtime security monitoring
- **RBAC Manager** - Simplify Kubernetes RBAC policies
- **Cloudflare Origin CA Issuer** - Cloudflare certificate integration
- **AWS Private CA Issuer** - AWS Private CA management

#### Observability & Monitoring
- **Insights Agent** - Cluster health insights
- **Datadog Agent** - Kubernetes monitoring and APM
- **Datadog Synthetics Private Location** - Synthetic monitoring for reliability
- **Prometheus Stack** - Open-source metrics monitoring
- **Metrics Server** - Resource usage monitoring
- **OTEL Operator** - Open Telemetry integration

#### Scaling & Cost Optimization
- **Karpenter** - Automated Kubernetes node scaling
- **Cluster Autoscaler** - Scale nodes dynamically
- **Keda** - Event-driven autoscaling
- **VPA** - Vertical Pod Autoscaler
- **Goldilocks** - Optimize resource requests and limits
- **Ocean Kubernetes Controller** - Spot instance management

#### CI/CD & Workload Management
- **Argo CD** - GitOps continuous deployment
- **Helm Release Pruner** - Cleanup outdated Helm releases
- **Gitlab Runner** - Run CI/CD jobs on Kubernetes

#### Storage & Persistent Volumes
- **AWS EBS CSI Driver** - Manage EBS volumes in Kubernetes
- **AWS EFS CSI Driver** - Manage EFS volumes in Kubernetes
- **Docker Registry** - Container registry for Kubernetes

#### Maintenance & Upgrades
- **kured** - Automated Kubernetes node reboots
- **Telepresence** - Simplify local Kubernetes development
- **Gloo** - API gateway and service mesh solutions 

We welcome your input. If you have feedback, please submit an issue.

## Requirements

Fairwinds Elements assumes the existence of Kubernetes, the necessity or value of various components of Fairwinds Elements will change based on where the Kubernetes cluster is running (AWS vs. GCP or Azure vs. Datacenter etc...). Fairwinds Elements can be leveraged as individual components, or together as a whole. 

**Not there yet? For a service involving setting up Kubernetes and installing all of these components out of the box, get in touch with Fairwinds.**
