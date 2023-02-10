# Task2.-K8S

Using K8S cluster that was created at the previous [Home Task](https://github.com/Heckfy05/Task1.-K8S) running on GCP.
1. Get information about your worker node and save it in some file
   >kubectl describe nodes kubenode > NodeInfo.txt

[File](https://github.com/Heckfy05/Task2.-K8S/blob/main/NodeInfo.txt) with the information about node.

2. Creating a new namespace (homework2) all resources will be created in homework2 namespace
![namespace creating](https://github.com/Heckfy05/Task2.-K8S/blob/main/img/namespace.jpeg?raw=true)

3. Preparing [deployment.yaml]() file that will create a Deployment with 3 pods of Nginx and service for access to these pods via ClusterIP and NodePort. 



Show the status of deployment, pods and services. Describe all resources which you will create and logs from pods
