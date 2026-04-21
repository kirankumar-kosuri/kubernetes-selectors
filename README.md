# Kubernetes Selectors

This repository provides hands-on examples and explanations of **Kubernetes Selectors**, one of the core concepts used to organize and manage resources in a Kubernetes cluster.

## What are Selectors?

Selectors are used to **filter and identify Kubernetes resources** based on labels. They help in grouping resources and performing operations on specific sets of objects.

- Labels → Key-value pairs attached to resources
- Selectors → Queries used to filter resources based on labels

Selectors act as a bridge between different Kubernetes objects like **Pods, Services, and Deployments**. :contentReference[oaicite:0]{index=0}

---

## Types of Selectors

### 1. Equality-Based Selectors
Used to match resources based on equality conditions.

**Operators:**
- `=`
- `==`
- `!=`

**Example:**
```bash
kubectl get pods -l app=nginx
kubectl get pods -l env!=prod
