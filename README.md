# My Private Cloud Project

## Introduction
In the era of digital transformation, cloud computing has become a cornerstone for delivering flexible, scalable, and cost-efficient IT infrastructure. Among the various cloud deployment models, Private Cloud stands out as a solution that offers dedicated resources to a single organization. This approach provides complete control over infrastructure, greater customization, and enhanced security, making it particularly suitable for businesses with strict compliance requirements or sensitive workloads.

Private Cloud environments can be deployed on-premises or in dedicated data centers, enabling organizations to proactively manage performance, capacity, and data governance. Unlike public cloud, where resources are shared among multiple tenants, a private setup ensures predictable performance and tailored configurations aligned with organizational policies.

To build and operate such an environment efficiently, OpenStack has emerged as one of the most widely adopted open-source platforms. It enables the creation and management of Infrastructure-as-a-Service (IaaS) by orchestrating compute, storage, and networking resources through a unified control plane. OpenStack’s modular architecture, extensive API support, and active community development make it highly adaptable—supporting deployments that range from small laboratory setups to enterprise-scale cloud infrastructures.

With these advantages, deploying a Private Cloud using OpenStack provides both the flexibility of modern cloud computing and the security of dedicated infrastructure. This project aims to implement such a system in a controlled environment to explore its capabilities, operational workflows, and scalability potential.

## Objectives:
In this project, a Private Cloud system will be deployed on Ubuntu 22.04 with a scale of 1–2 nodes, ensuring the following core capabilities:
- Manage, create, delete, and modify virtual machines (VMs).
- Create, delete, modify, and configure virtual networking.
- Integrate and operate a Block Storage system within the OpenStack environment.

## Infrastructure:
<img width="600" height="500" alt="image" src="https://github.com/user-attachments/assets/00066472-8923-471b-a3f7-031e4887b863" />

## Openstack components:
In this Private Cloud deployment, the following OpenStack services are implemented:
Keystone – Identity service that manages authentication and authorization across OpenStack.
Glance – Image service used to store and retrieve VM disk images.
Nova – Compute service responsible for creating and managing virtual machines.
Placement – Tracks resource inventories and usage for efficient scheduling of VMs.
Neutron – Networking service that provides connectivity between interface devices managed by other OpenStack services.
Cinder – Block Storage service that provides persistent volumes for virtual machines (using LVM backend).
Horizon – Web-based dashboard for managing and monitoring cloud resources.
MariaDB – Relational database for storing service configurations and operational data.
RabbitMQ – Message broker for communication between services.
Apache2 – Web server that serves APIs and the Horizon dashboard.
