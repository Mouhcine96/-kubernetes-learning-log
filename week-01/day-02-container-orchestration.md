# Day 02 – Container Orchestration

## Core idea
Container orchestration manages containers across multiple hosts to provide scalability,
fault tolerance, and automation.

## Why this matters
Running containers on a single host does not scale and creates single points of failure.
Orchestrators like Kubernetes automate restarts, placement, and scaling.

## Key takeaway
Containers package applications.
Orchestrators operate systems.

## Containers – recap

- Containers are isolated processes sharing the host OS kernel.
- They package applications together with their dependencies.
- Container images are immutable templates.
- Containers are running instances of images.

## What is container orchestration?

Running containers on a single host can be sufficient for development.
In QA and production this breaks down quickly.

Production systems require:
- Fault tolerance
- On-demand scalability
- Efficient resource usage
- Service discovery
- External access
- Zero-downtime updates and rollbacks

Container orchestrators group multiple hosts into a cluster and automate
the deployment and lifecycle of containers at scale.

This turns containers into a distributed system with better reliability,
performance, and cost efficiency.

## Container orchestration tools – overview

There are many container orchestrators, often tied to specific cloud vendors.

- ECS / ACI: Managed, cloud-specific solutions
- Docker Swarm: Deprecated in practice
- Nomad: Niche orchestrator, often used with HashiCorp tools
- Kubernetes: Open-source standard, CNCF project, widely adopted

## Key takeaway
Kubernetes is the industry standard for container orchestration.
Most other solutions are either vendor-locked or niche.
