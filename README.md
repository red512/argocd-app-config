# argocd-app-config
Description
This project uses Argo CD to deploy a simple Python server using Kubernetes. It consists of three YAML files, deployment.yaml, service.yaml, and application.yaml, which define the deployment, service, and application specifications respectively.

The `deployment.yaml` file specifies the deployment of a containerized Python server, with two replicas and exposed on port 8080.

The `service.yaml` file creates a Kubernetes service for the deployment, which routes traffic to the pods running the Python server. The service listens on port 8080.

The `application.yaml` file defines the Argo CD application for this deployment. It specifies the source of the configuration (a GitHub repository), the destination (the Kubernetes cluster), and the sync policy (to create the namespace if it does not exist and enable automated self-healing and pruning).

Usage
To deploy this project using Argo CD, first create a new project in Argo CD, and then create a new application in the project. Use the application.yaml file as the application specification, and Argo CD will take care of deploying the Python server to your Kubernetes cluster.

Credits
This project was created by red512 and is intended for educational purposes only.
