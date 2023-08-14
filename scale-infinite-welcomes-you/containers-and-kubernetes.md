# Containers and Kubernetes

**Containers :**

* A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. A Docker container image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.
* Container images become containers at runtime. Containers isolate software from its environment and ensure that it works uniformly despite differences for instance between development and staging.

**Virtual machines vs Containers :**



<figure><img src="../.gitbook/assets/container.png" alt=""><figcaption></figcaption></figure>

**Kubernetes :**

Kubernetes is an open-source container-orchestration system for automating deployment, scaling, and management of containerized applications. It has a large, rapidly growing ecosystem and the services, support, and tools are widely available. Kubernetes provides you with a framework to run distributed systems resiliently.



<figure><img src="../.gitbook/assets/kubernetes.png" alt=""><figcaption></figcaption></figure>

A Kubernetes cluster consists of a set of worker machines, called nodes, that run containerized applications. Every cluster has at least one worker node.

The worker node(s) host the Pods that are the components of the application workload. The control plane manages the worker nodes and the Pods in the cluster. In production environments, the control plane usually runs across multiple computers and a cluster usually runs multiple nodes, providing fault-tolerance and high availability.

**Kubernetes Benefits :**

* Extreme Scaling - Due to its decoupled architecture support, Kubernetes provide a different kind of scaling for various purposes. For scaling of servers, you can use horizontal scaling, for the containers auto and manual scaling can be used, and for pods, you can use the replication controller.
* Enhanced Deployment Speed - You can continuously update your applications without any downtime. It supports features like immutable infrastructure, self-healing, and declarative configuration.
* High Availability - Kubernetes is designed to handle both the application and infrastructure. With its auto replacement feature, it can replace or heal any crashed pod. It can automatically balance the network load with its in-built load balancers.
* Portability - Kubernetes supports several platforms. You can run it on any public cloud, on-premises, and even multi-cloud. Due to its high flexibility, you can use it in any environment.
* Security - All the confidential information, for example, passwords, OAuth tokens, and SSH keys are stored securely on the Kubernetes secret object. You can easily replace the stored data without exposing it.
