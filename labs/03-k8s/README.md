# ☸️ Kubernetes / OpenShift overview

In this section we will explore the core component of a Kubernetes cluster. Even if the lab
is built on OpenShift, the exact same concepts apply to all Kubernetes distributions.

> **NOTE:** For the Cloud-based distro (i.e. GKE, AWS EKS, etc.) the control-plane is often hosted & managed by the cloud provider.
> Therefore you can not always see the same results as with self-hosted flavor.

## What is my cluster made of ?

`kubectl` is the command-line tool for interacting with and managing Kubernetes clusters.

`oc` is the OpenShift equivalent. It includes all `kubectl` commands plus OpenShift-specific features like project management, OAuth login, and debugging.

Let's see what's available:
```bash
oc get nodes
```

Get the list of nodes with their status:
```bash
oc get nodes -o wide
```

The `STATUS` columns gives a summarized view of what node "health".
Popular status are `Ready`, `NotReady` and `SchedulingDisabled`.

> **NOTE:** The `-o wide` is available for most `get [resource]` and give you more information.

Get the list the nodes with their labels:
```bash
oc get nodes -o wide --show-labels
```

The `LABELS` columns gives information about the node such as the memory size, number of CPUs, etc.


