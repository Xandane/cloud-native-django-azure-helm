# Kubernetes ToDo Application with Helm Charts

## Overview

This project implements a cloud-native ToDo application deployed on a Kubernetes cluster using Helm charts. It demonstrates infrastructure automation, Kubernetes resource management, and application packaging using Helm.

The system consists of:
- ToDo application deployed via Helm
- MySQL database deployed as a Helm subchart
- Fully configurable Kubernetes resources via values.yaml
- Automated deployment using kind cluster

---

## Architecture

- Kubernetes cluster (kind)
- Helm-based application deployment
- ToDo application (frontend + backend)
- MySQL database (Helm subchart)
- Persistent Volumes (PV/PVC)
- Horizontal Pod Autoscaler (HPA)
- Configurable secrets and environment variables

---

## Features

- Helm-based deployment of full application stack
- Separate MySQL subchart with dependency management
- Fully configurable values.yaml for all resources
- Secrets managed via Helm templating (range function)
- Resource limits and requests configurable per environment
- Node affinity and tolerations support
- HPA for autoscaling based on CPU and memory
- Persistent storage configuration via Helm
- Automated deployment using bootstrap script

---

## Tech Stack

- Kubernetes (kind cluster)
- Helm 3
- Docker
- Bash scripting
- MySQL
- Linux environment

---

## Deployment

### Prerequisites

- kind cluster installed
- kubectl installed
- helm installed

---

### Deploy Application

```bash
./bootstrap.sh
