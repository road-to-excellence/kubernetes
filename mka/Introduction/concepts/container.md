### Containers
---
***CONTAINER IMAGES*** - A container image is a ready-to-run software package containing everything needed to run an application

***CONTAINER RUNTIMES*** - These are runtimes (such as containerd, etc.) that are used to run containers efficiently. It also supports custom implementations of the Kubernetes CRI (Container Runtime Interfaces) as well. [More configuration can be read here](https://kubernetes.io/docs/concepts/containers/runtime-class/)

***CONTAINER ENVIRONMENT*** - These are default and custom runtime important resources provided to the container at runtime.
- A filesystem, which is a combination of an image and one or more volumes.
- Information about the Container itself.
- Information about other objects in the cluster.
    [READ MORE...](https://kubernetes.io/docs/concepts/containers/container-environment/)

***CONTAINER LIFECYCLE HOOKS*** - There are two hooks that are exposed to Containers:
1. PostStart
2. PreStop

For more detailed information [READ MORE...](https://kubernetes.io/docs/concepts/containers/container-lifecycle-hooks/)

