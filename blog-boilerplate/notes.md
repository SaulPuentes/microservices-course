# Kubernetes Notes

## Types of Services

- **Cluster IP**: Sets up an easy URL to access a pod. Only exposes pods _in the cluster_.

- **Node Port**: Makes a pod accessible from _outside the cluster_. Usually only used for dev purposes.

- **Load Balancer**: Makes a pod accessible from _outside the cluster_. This is the right way to expose a pod to the outside world.

- **External Name**: Redirects an in-cluster request to a CNAME url.

## Commands

Get the node port to access to the service in the browser.

```console
foo@bar:~$ kubectl describe service posts-srv
```
