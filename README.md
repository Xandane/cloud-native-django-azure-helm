# Kubernetes ToDo Application with Helm Charts

## Overview

This project implements a cloud-native ToDo application deployed on a Kubernetes cluster using Helm charts. It demonstrates infrastructure automation, Kubernetes resource management, and Helm-based application packaging.

The application stack includes:

- ToDo web application
- MySQL database deployed as a Helm subchart
- Kubernetes Persistent Volumes (PV/PVC)
- Horizontal Pod Autoscaler (HPA)
- Configurable deployment via Helm values
- Automated deployment using a bootstrap script

---

## Architecture

The project uses a Kubernetes-based architecture with Helm-managed resources.

Components:

- Kubernetes cluster (`kind`)
- Helm charts for deployment management
- Django ToDo application
- MySQL StatefulSet
- Persistent storage (PV/PVC)
- Horizontal Pod Autoscaler (HPA)
- RBAC and Service Accounts
- Configurable secrets and environment variables

---

## Features

- Helm-based deployment of the entire application stack
- Separate MySQL subchart with dependency management
- Fully configurable `values.yaml`
- Kubernetes secrets managed through Helm templating
- Configurable CPU and memory limits/requests
- Node affinity and tolerations support
- Horizontal Pod Autoscaler configuration
- Persistent storage configuration
- Automated deployment workflow using `bootstrap.sh`
- Infrastructure organized in reusable Kubernetes manifests

---

## Tech Stack

- Kubernetes (`kind`)
- Helm 3
- Docker
- Django
- MySQL
- Bash scripting
- YAML
- Linux environment

---

## Project Structure

```text
.
├── .infrastructure/
├── helm-chart/
│   └── todoapp/
│       └── charts/mysql/
├── src/
├── bootstrap.sh
├── cluster.yml
├── README.md
└── docs/