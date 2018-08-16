# Cloud Computing

### **What is Cloud Computing**

Cloud computing is a general term that services are hosted over the internet. It enables companies to consume the data storages, computing powers as the utility, and eliminates the management of intricate underlying infrastructure and configuration.

### **Why do we use Cloud Computing**

Comparing with the past, developers buy bare-metal hardwares and install servers in their private cloud, which is the on-premises model where developers have the full control of whole infrastructure. However, companies still need to pay the utilities as well as maintenance cost even if no one is using the service or the service is not popular to justify the cost. Nowadays, these hardwares can be maintained by cloud providers and share with multiple tenants by virtual of virtualization. Users just need to pay the on-demand price and don’t need to worry about the underlying hardware, networking, and utility configuration. As a result, it’s more cost effective and ease of DevOps operations.

### **Different Categories of Cloud Computing**

Typically, depending on the various needs, there are five models for the cloud services : IaaS, Caas, Paas, FaaS, SaaS. The more left, the more flexible it is, which means developers can be more capability to customize their services and manage the underlying servers.

![Key differences between IaaS, PaaS, SaaS, Source \[5\]](https://lh3.googleusercontent.com/xxIRKuKjnje_q_ahkXpqSkYCamfolezCIH2xA9uhEfmFFvJqQ6bioE20c4k-Ga01dKui6mr4ezu6k60kbaQdXoLjExcE3QTT3IZHjNiDf2wc6cjchz4pRRbxXYnKxBJhtXdRaLp1)

#### **Infrastructure as a Service \(IaaS\)**

IaaS allows developers to run their services on cloud environment with monitoring, accessing, and controlling the computing instances, storages, and networking. Developers can choose whatever runtime they want and install or configure the softwares. The computing resources can be purchased on-demand, while the cloud provider manages the underlying hardwares.

Example: Amazon Web Services, Google Cloud Platform, Microsoft Azure

#### **Container as a Server \(CaaS\)**

CaaS offers an easy way to deploy their services in a container cluster. Typically, developers put the software dependencies in a docker container image, and deploy them in the Kubernetes orchestration.

Example:Amazon Elastic Container Service, Google Kubernetes Engine, Azure Container Service

#### **Platform as a Service \(PaaS\)**

PaaS provides a way where developers can customize their applications based on their needs, but the servers, storages, and networking are managed by the cloud provider.

Example: Google App Engine, Heroku

#### **Function as a service \(FaaS\)**

Function as a service \(FaaS\) platform is a compute runtime to execute the program logics without storing data, which is based on event-driven programming model. The first commercial product of FaaS was Zimki in 2006, which was not quite successful at that time. Then, Google launched the Google App Engine \(GAE\) in 2008. The AWS lambda was introduced by Amazon in 2014, which is a popular FaaS platform. Oracle introduced Fn. IBM published OpenWhisk as an open source serverless framework. Microsoft provided Azure function.

Example: AWS Lambda, Google Cloud Functions, Azure Function, Fission, Kubeless, Funktion, OpenWhisk

#### **Software as a Service \(SaaS\)**

SaaS application provides service over the Internet on the cloud environment, users don’t have to download or install it into their computers. Developers host their services on cloud providers, and they don’t have the permission to change the underlying configuration of servers.

Example: GMail, Spotify Music

Nowadays, developers need a fast way to verify their ideas and address the dynamic loads coming from users requests as well. Therefore, the serverless programming can be a cost effective and quick way to achieve this goal. Next, the concept of serverless programming will be discussed in detail, and several open source projects will be compared for you to reference.

  
  


