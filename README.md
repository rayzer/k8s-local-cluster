# Kubernetes cluster
A vagrant script for setting up a Kubernetes cluster using Kubeadm.

Modified to suit my own network situation by using aliyun mirror instead.

And including fix for missing /etc/default/kubelet.


## How to Run

Execute the following vagrant command to start a new Kubernetes cluster, this will start one master and two nodes:

```
vagrant up
```

You can also start invidual machines by vagrant up k8s-head, vagrant up k8s-node-1 and vagrant up k8s-node-2


## Clean-up

Execute the following command to remove the virtual machines created for the Kubernetes cluster.
```
vagrant destroy -f
```

You can destroy individual machines by vagrant destroy k8s-node-1 -f
