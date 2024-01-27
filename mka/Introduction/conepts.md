## Concepts

To learn about the concepts properly. The document ([Kubernetes Concepts](https://kubernetes.io/docs/concepts/)) from [kubernetes.io](https://kubernetes.io) is recommended

### 1. Cluster Architecture

![Clust_Arch](/mka/images/introduction/cluster_arch.png "Kubernetes Cluster Architecture")

***NODES*** - These are also referred to as worker in master-worker architecture. These are the core machines (or VMs) where user load runs. Other than user load, nodes include **kubelet**, **container runtime** and **kube-proxy** as base components. ***[Click here to know more on Nodes.](https://kubernetes.io/docs/concepts/architecture/nodes/)***

***NODES - CONTROL PLANE [COMMUNICATION]*** - ***[Click here to read about the internal communication between Nodes and Control Plane.](https://kubernetes.io/docs/concepts/architecture/control-plane-node-communication/)*** (Not recommended unless you need to get a very deep, network level, understanding between nodes and control plane.)

***CONTROLLERS*** - In K8s, these are control loops that watches the state of cluster currently and tries to bring back them closer to the desired state. ***[Click here to know more on Controllers.](https://kubernetes.io/docs/concepts/architecture/controller/)***

***LEASES*** - Leases are the requirement of every distributed system to manage shared resources. These are objects created under api group `coordination.k8s.io`. These are used for system-critical capabilities such as node heartbeat, component level leader election, etc. ***[Click here to know more on Leases.](https://kubernetes.io/docs/concepts/architecture/leases/)***

***CLOUD CONTROLLER MANAGER*** - This is a type of controller manager that provides the Cloud Service providers to manage some of the cluster resources (such as Nodes, Routes, Services, etc) using their own APIs (Cloud provider's API). ***[Click here to know more on Cloud Controller Manager.](https://kubernetes.io/docs/concepts/architecture/cloud-controller/)***

***CGROUP (CONTROL GROUP V2)*** - Since this is valid for Linux distribution. ***[Click here to know about CGROUPv2.](https://kubernetes.io/docs/concepts/architecture/cgroups/)***

***CONTAINER RUNTIME INTERFACE (CRI)*** - It is a protocol (similar to API) used between kubelet and container runtime. ***[Click here to know more about CRI.](https://kubernetes.io/docs/concepts/architecture/cri/)***

***GARBAGE COLLECTION*** - This is a deep topic discussing about how and what are the cleanup procedures kubernetes follow. ***[Click here to read about Garbage Collection in Kubernetes.](https://kubernetes.io/docs/concepts/architecture/garbage-collection/)***

***MIXED VERSION PROXY*** - As the name suggests it a proxy between multiple server, here API Servers. This allows the Kubernetes API Server to proxy between peers API Server for resource creation and query. ***[Click here to know about Mixed Version Proxy](https://kubernetes.io/docs/concepts/architecture/mixed-version-proxy/)***