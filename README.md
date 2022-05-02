# router-sidecar

* The Slice Router is a network service component that provides a virtual L3 IP routing functionality within a cluster for the Slice overla network.
* Each slice in a cluster has one slice router with the possibility of a redundant pair option. 
* The Slice Operator manages the lifecycle of a Slice Router by overseeing the deployment, configuration,  continuous monitoring, and management of the Slice Router.
* The Slice Router provides a full mesh network connectivity between the application pods and slice gateway pods in a cluster. 

## Getting Started

It is strongly recommended to use a released version.

### Prerequisites

* Docker installed and running in your local machine
* A running [`kind`](https://kind.sigs.k8s.io/) or [`Docker Desktop Kubernetes`](https://docs.docker.com/desktop/kubernetes/)
  cluster 
* [`kubectl`](https://kubernetes.io/docs/tasks/tools/) installed and configured

### Usages
You can use the command below to view all the slice routers in a cluster:

```bash
kubectl get pods -n avesha-system | grep vl3-nse-* 
```

## License

This project is released under the Apache 2.0 License.
