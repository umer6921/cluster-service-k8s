# Services in Kubernetes
## What is services?
In Kubernetes, a "Service" is like a traffic cop for your applications. It helps manage how different parts of your application talk to each other, and it can also make your application available to the outside world. There are four types of services 

1) ClusterIP (By default)
2) NodePort
3) LoadBalancing
4) HeadLess

## ClusterIP?
ClusterIP is employed for inter-pod communication across various nodes within the identical cluster, assigning a virtual IP to the cluster itself, which pods can then utilize for their communication needs. 

## NodePort?
NodePort is a way to make your applications in Kubernetes reachable from outside the cluster, allowing people or services on the internet to access your web applications or services running inside the cluster. 

![image](https://github.com/umer6921/cluster-service-k8s/assets/75561123/4c57fa4c-303a-4308-93f3-7bc3bad3ab24)


## Why to use services?
Services offer a solution for the dynamic nature of Pods' IP addresses within Kubernetes. Instead of dealing with the complexity of dynamic IP assignments where Pods can change their IP addresses, Services provide a stable and unchanging IP address that you can use to reliably access your Pods. This means that even if a Pod fails and is replaced with a new one, the Service ensures that you can consistently reach your application components using a single, static IP address.
