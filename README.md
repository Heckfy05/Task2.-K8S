# Task2.-K8S

Using K8S cluster that was created at the previous [Home Task](https://github.com/Heckfy05/Task1.-K8S) running on GCP.
1. Get information about your worker node and save it in some file
   >kubectl describe nodes kubenode > NodeInfo.txt

[File](https://github.com/Heckfy05/Task2.-K8S/blob/main/NodeInfo.txt) with the information about node.

2. Creating a new namespace (homework2) all resources will be created in homework2 namespace
![namespace creating](https://github.com/Heckfy05/Task2.-K8S/blob/main/img/namespace.jpeg?raw=true)

3. Preparing [deployment.yaml](https://github.com/Heckfy05/Task2.-K8S/blob/main/deployment.ymal) file that will create a Deployment with 3 pods of Nginx and service for access to these pods via ClusterIP and NodePort.
As resoults of deploying:
![dep](img/CreatingDepPodSRC.png)
Status of the deployment, pods and services:
![status](img/GetInfo.png)

[Description](NodeDescription.txt) of the Node
>kubectl describe nodes kubenode -n homework2 > NodeDescribe.txt

[Description](DescribePods.txt) of the Pod's
>kubectl describe pods -n homework2 > DescribePods.txt

[Description](DescribeServices.txt) of the Services
>kubectl describe service -n homework2 > DescribeServices.txt

Logs from Pods:
![LogsPods](img/PodsLogs.png)

