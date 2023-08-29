# Services in Kubernetes
## What is services?
In Kubernetes, a "Service" is like a traffic cop for your applications. It helps manage how different parts of your application talk to each other, and it can also make your application available to the outside world. There are four types of services 

1) ClusterIP (By default)
2) NodePort
3) LoadBalancing
4) HeadLess

ClusrerIP is used to communicate between pods from different nodes within the same cluster. It gives virtual IP to the cluster and the pods can use the VIP to communicate. 

## Why to use services?
Services offer a solution for the dynamic nature of Pods' IP addresses within Kubernetes. Instead of dealing with the complexity of dynamic IP assignments where Pods can change their IP addresses, Services provide a stable and unchanging IP address that you can use to reliably access your Pods. This means that even if a Pod fails and is replaced with a new one, the Service ensures that you can consistently reach your application components using a single, static IP address.
