# MLOps-Kubernetes
A repository for a ML project on Kubernetes

##Deploying Machine Learning Models on Kubernetes
A common pattern for deploying Machine Learning (ML) models into production environments - e.g. ML models trained using the SciKit Learn or Keras packages (for Python), that are ready to provide predictions on new data - is to expose these ML as RESTful API microservices, hosted from within Docker containers. These can then deployed to a cloud environment for handling everything required for maintaining continuous availability - e.g. fault-tolerance, auto-scaling, load balancing and rolling service updates.

The configuration details for a continuously available cloud deployment are specific to the targeted cloud provider(s) - e.g. the deployment process and topology for Amazon Web Services is not the same as that for Microsoft Azure, which in-turn is not the same as that for Google Cloud Platform. This constitutes knowledge that needs to be acquired for every cloud provider. Furthermore, it is difficult (some would say near impossible) to test entire deployment strategies locally, which makes issues such as networking hard to debug.

Kubernetes is a container orchestration platform that seeks to address these issues. Briefly, it provides a mechanism for defining entire microservice-based application deployment topologies and their service-level requirements for maintaining continuous availability. It is agnostic to the targeted cloud provider, can be run on-premises and even locally on your laptop - all that's required is a cluster of virtual machines running Kubernetes - i.e. a Kubernetes cluster.


Work based on the following repo: AlexIoannides/kubernetes-mlops
