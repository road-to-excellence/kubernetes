## Why Kubernetes?

Althouh below will answer the query, still this is a good read blog - [Why should you use Kubernetes?](https://www.softwareone.com/en/blog/articles/2021/03/23/why-kubernetes-2022)

#### 1. Service discovery and load balancing
- Kubernetes can expose a container using the DNS name or using their own IP address. If traffic to a container is high, Kubernetes is able to load balance and distribute the network traffic so that the deployment is stable.
#### 2. Storage orchestration
- Kubernetes allows you to automatically mount a storage system of your choice, such as local storages, public cloud providers, and more.
#### 3. Automated rollouts and rollbacks
- You can describe the desired state for your deployed containers using Kubernetes, and it can change the actual state to the desired state at a controlled rate. For example, you can automate Kubernetes to create new containers for your deployment, remove existing containers and adopt all their resources to the new container.
#### 4. Automatic bin packing
- You provide Kubernetes with a cluster of nodes that it can use to run containerized tasks. You tell Kubernetes how much CPU and memory (RAM) each container needs. Kubernetes can fit containers onto your nodes to make the best use of your resources.
#### 5. Self-healing
- Kubernetes restarts containers that fail, replaces containers, kills containers that don't respond to your user-defined health check, and doesn't advertise them to clients until they are ready to serve.
#### 6. Secret and configuration management
- Kubernetes lets you store and manage sensitive information, such as passwords, OAuth tokens, and SSH keys. You can deploy and update secrets and application configuration without rebuilding your container images, and without exposing secrets in your stack configuration.
#### 7. Batch execution 
- In addition to services, Kubernetes can manage your batch and CI workloads, replacing containers that fail, if desired.
#### 8. Horizontal scaling
- Scale your application up and down with a simple command, with a UI, or automatically based on CPU usage.
#### 9. IPv4/IPv6 dual-stack
- Allocation of IPv4 and IPv6 addresses to Pods and Services
#### 10. Designed for extensibility
- Add features to your Kubernetes cluster without changing upstream source code.