## Introduction to Kubernetes

Kubernetes is container orchestration tool.
Kubernetes, also known as K8s, is a portable open source platform — with a rapidly growing ecosystem — for managing containerized workloads and services. Kubernetes aids declarative configuration, automates deployment, and manages cloud native applications with on-premise systems or public cloud infrastructure.

#### What does container orchestration tool do?

1. High Availability / No Downtime
2. Scalability / High Performance
3. Disaster Recovery - backup and restore

### Basic Architecture

1. Atleast 1 master node connected to one or more worker nodes.
2. Each worker node has `kubelet` process running on it.
3. Each worker have docker containers running on it.
4. Worker is actual location of running apps.
5. Master runs `kubernetes processes` required to run and manage cluster. Example - `API SERVER`, `CONTROLLER MANAGER`

### Different parts explanation

##### API SERVER
Server used as entrypoint to cluster. Used either via UI, API or CLI(`kubectl`)

##### CONTROLLER MANAGER
Keeps tracks of what's happening in the cluster.

##### SCHEDULER
Responsible for Scheduling of Pods onto the cluster.

##### ETCD
Key value storage. Stores current state of kubernetes cluster.

##### VIRTUAL NETWORK
Used to connect all nodes (worker and master).

### Basic Concepts

##### POD & CONTAINERS
Pod is a smallest unit controlled by a user. It manages the containers.
A worker can have multiple pod and a pod can have a multiple container.
These usually holds one application per pod.
Each Pod gets it's own IP Address.

##### SERVICE
Since Pods are dynamic and can have new IP Address once Pod is restarted.
To overcome that, we use services. These are permanent IP Address and a Load Balancer for a Pod.

##### DEPLOYMENTS
A template for creating pods.
```
kind: Deployment
spec:
  template:
    // POD TEMPLATE
```
***CONTROLLER MANAGER TASK*** - Check desired and actual state and take action.
