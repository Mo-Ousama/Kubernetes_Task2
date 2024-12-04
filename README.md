# Kubernetes_Task2
1- How many Namespaces exist on the system?
2- How many pods exist in the kube-system namespace?
3- Create a deployment with
Name: beta
Image: redis
Replicas: 2
Namespace: finance
Resources Requests:
CPU: .5 vcpu
Mem: 1G
Resources Limits:
CPU: 1 vcpu
Mem: 2G
4- How many Nodes exist on the system?
5- Do you see any taints on master?
6- Apply a label color=blue to the master node
7- Create a new deployment named blue with the nginx image and 3 replicas
Set Node Affinity to the deployment to place the pods on master only
NodeAffinity: requiredDuringSchedulingIgnoredDuringExecution
Key: color
values: blue
