## Workloads

***BRIEF*** - <br>
A workload can be of multiple / single application (AKA components) working together (in K8s, these run in a pod).<br>
However, the pod management could be challenging, so k8s makes the users life easier by introducing multiple workload resources, which deals with controller to manage the right number and state of pods.

These workload resources are as follows -
1. Deployment & ReplicaSet
2. Statefulset
3. Daemonset
4. Job & Cronjob

Let's see all these workloads one by one.

### Pods

Smallest deployable unit that can be manageable by a user in k8s.
<!---@include:../concepts.md--->

### Deployments

