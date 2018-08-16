# Serverless Programming

### **What is Serverless Programming**

#### **Introduction**

Serverless programming \(serverless computing\) is a computation model offered by the cloud provider where the orchestration of computing resources are dynamically allocated by them according to the needs. The fees are determined by how much on-demand computing resource you used instead of the predetermined pricing of the computing units.

The name of Serverless might not be accurate. In fact, it still need the servers hosted to provide services. However, instead of managing the underlying infractures, the management of these servers are taken care by the cloud provider. As a result, the developers and operators don’t need to worry about the intricate settings behind the scene.

Before diving into the serverless programming, it might be helpful to understand how developers deploy their services in the past.

#### **Moving from Microservices to FaaS**

Microservices is a form of Service-oriented Architecture where a monolithic application is splitted into multiple microservices. It helps services to be scalable on the cloud platform, such as Amazon AWS, Google GCP, Microsoft Azure, or Kubernetes. Since each service can operate independently, they don't need to rely on each other to function. Besides, each of them may have their own development environment and can be deployed or scaled based on their own decisions. FaaS can be deployed on microservices as well where the developers no need to take care of operations and orchestration of servers. Here, FaaS can be used to achieve serverless computing.  
****

![FaaS in MicroServices](https://docs.google.com/a/west.cmu.edu/drawings/d/spGEWym3QK98N5WB_XlUFLw/image?w=444&h=196&rev=173&ac=1&parent=1EUsG35X6sKJWvdjt7U5mYhX2NKF0AWytOH5c6mLz6O0)

Although there are quite a lot of commercial versions of serverless computing, there still are many outstanding open source projects that can be used in production environment. These open source frameworks can be more useful in terms of flexibility and customization. In order to set up the serverless computing environment, kubernetes can be a reliable system for management of containerized application, ease of deployment, and auto-scaling stuff as a cloud platform. It can easily combined with docker to provide os-level virtual computing environment on servers. Then, we can use serverless function framework on top of Kubernetes to provide services. In the following section, this article will introduce multiple frameworks, compare them in terms of pros and cons, and then give out our suggestions for various situations.

#### **Why do we use Serverless Programming**

Nowadays, developers need a way to verify their idea fastly and address the dynamic loads coming from requests of users. Serverless programming can ease the pain of configuration of deployment, management of underlying infrastructure, and automatically scaling services. Therefore, developers are able to only focus on their idea realization and spend more time to verify it.

Here, the pros and cons are listed in the following sections for users to consider.

**Advantages**

* Ease of operation
  * Developers don’t have to worry about the setting of programming environment and orchestration of resource to address the dynamic loading of the service. The cloud provider helps you take care of underlying infrastructure and patches for essential components.
* High Scalability
  * The cloud provider would help you scale in or out your service based on the request and loading of your service.
* Low Cost
  * Traditionally, developers need to rent a server or self-owned a private cloud, they need to pay the fixed utility and upfront fees even if no users are using their services. However, with serverless computing they just need to pay the amount of money associated with the requests generated by users, which is pay-as-you-go pricing model offered by cloud provider.

**Disadvantages**

* Low Customization
  * Since the servers are hosted by cloud providers, they need to offer a solution that fits the general situation, while minimize the risks or security concerns. As a result, the flexibility for customization might be a problem. For example, on Google App Engine \(GAE\), developers could not use c-extension related modules in python, like numpy. Besides, it is not suitable for high-performance computing, because the servers are shared by multiple tenants at the same time. Typically, you can not change the network bandwidth, computing power, and memory capacity once it is decided by provision in advance.
* Unstable Performance
  * Resources are shared by multiple tenants at the same time. Although virtual environment can be used to prevent heavy users from affecting others, sometimes there still are variations in terms of performance. In addition, when your application go viral, it needs more resources to address the peak requests, but sometimes it needs time to warm up the computing instances and prepare the resource, which might not be able to address the peak traffic in time.
* Privacy Concern
  * The customer data and code resides on the cloud environment hosted by cloud providers, it might incur some privacy concern to some companies in terms of sensitive data.

#### **Applications**

[Netflix uses AWS lambda service](https://aws.amazon.com/solutions/case-studies/netflix-and-aws-lambda/) to help manage the underlying AWS infrastructure with event-based systems.

#### **Use Cases**

1. Serving up static content

If you have static content to read or write, you can use the FaaS to help you scale up your service to address the dynamic loads. This is the simple and economic way to implement it.

![Source: medium.com \[6\]](https://lh6.googleusercontent.com/FrwofbHHOrbp9R0t888ZVeWsqmflI_znThZKV3ogSpkMLezxbrjiBw30CDuc2sy5sVB1oHb_AOR-JT_r5xx0182izProMEI3HM2Z7JpAk_SytI6IkMBkIkeCOTu8j0YFRHIkJLcg)

2. ETL \(Extract, Transform, Load\)

ETL process can be a heavy operation in your system. It takes a lot of resource and time to process it. However, with FaaS, it can help you run your functions depends on the event triggered by certain component, while you only need to pay for the amount of time that your program runs.

![Source: medium.com \[6\]](https://lh3.googleusercontent.com/IxMB2GOha_kzbKKB-hyki9RN7DR0yr6wfDfu5zxUkPi_Ld-Tz_JtFzB3Y-tQe71tuRboIxZSW0S52jmd-hCQ5KwCu94TPvKZywOYQyHKK3QyfDPX09immLFQKYYNIl_-bBL2IS-i)

3. Time based batch

The functions in FaaS can be scheduled in a way that is based on time or in sorted order. It is a simple way to do the scheduling jobs.

![Source: medium.com \[6\]](https://lh6.googleusercontent.com/8hLwS2ZvG3pUOrXs7ojXFAYZX9kM4cL69P2ZwfB2HdYG_1Pw0f-7tLwPfW3ZJFrxm5L50EuKBERWRpQ00VOapDGIAQVtR2IRxmNX9YoN1p-TvpKjETLqpLZttFBNtXIvmCRglhtN)

The area that might not work for Serverless Programming

1. The service that wants to configure the underlying infrastructure configuration that requires additional permission.  
2. The service that depends on the data from the specific machine.  
3. The service that may require additional packages or dependencies that not supported by the service provider. Like, c-extension library on python.

#### Different Categories of Serverless Programming

Serverless programming can be achieved by Function as a Server \(FaaS\).

#### Free and Open Source Resources

In this section, the free and open source resources will be listed.

* Articles
  * [OSSPal](http://osspal.org/project-categories/service-oriented-architecture-web-services)
  * [Awesome-Serverless](https://github.com/anaibol/awesome-serverless)
  * [Serverless Guide](https://github.com/serverless/guide)
* Books
  * [Serverless Computing: Current Trends and Open Problems](https://www.researchgate.net/publication/317557782_Serverless_Computing_Current_Trends_and_Open_Problems)
* Video training
  * [How a serverless platform is built on top of Containers: The Internals of Open Source Fn Project](https://www.youtube.com/watch?v=YgNrGT8pzYw)

#### Proprietary Resources

In this section, the proprietary resources will be listed.

* Articles
  * [Amazon AWS Lambda](https://aws.amazon.com/lambda/)
  * [Google Cloud Functions](https://cloud.google.com/functions/)
  * [Microsoft Azure Function](https://azure.microsoft.com/en-us/services/functions/?&OCID=AID719825_SEM_d6ITB4fz&lnkd=Google_Azure_Brand&gclid=EAIaIQobChMI3_mpoMDe3AIVxI5-Ch1fzwG8EAAYASAAEgIeIvD_BwE&dclid=CIaKiKHA3twCFYb0ZAodtIAMEg)
  * [Serverless Architectures](https://martinfowler.com/articles/serverless.html)
* Books
  * [AWS Lambda: A Guide to Serverless Microservices](https://www.amazon.com/AWS-Lambda-Guide-Serverless-Microservices-ebook/dp/B016JOMAEE)
* Video training
  * [Serverless Programming Solutions \[Video\]](https://www.packtpub.com/application-development/serverless-programming-solutions-video)

#### The major FLOSS tools/frameworks

The major FLOSS Tools/Framework open source projects of serverless programing include Fission, Kubeless, Funktion, and OpenWhisk.

![](https://lh3.googleusercontent.com/xOgEm6d4M0FbTzPEAw6rWxKvFbrXWbQjo4GNDAObMbPzQ9AUA0-NhfoycRUAUc1SkP2_2_mFoRiyKAqbIESrj6g0-WASNt-Ne44wsJJQ8-2eUg8Flwvz1C6KDyug58mn2iqqyBza)

Fission is a framework for serverless functions on Kubernetes introduced by Platform9. It is written by Go and focus on the productivity of developers and performance of services. Fission has small cold-start time about 100 msec due to the reason that each warm container contain a small dynamic loader, which helps to reduce the latency of start a function. It seamlessly combined with Kubernetes where users can monitor and do log aggregation of the services easily.

[Project Page](https://fission.io/)  
[Source Code](https://github.com/fission/fission)  
[License](https://www.apache.org/licenses/LICENSE-2.0)  
Platform  
OSSPal Link

![](https://lh3.googleusercontent.com/TMdf8b4Zwd_dULFnAXzKCP8FOI5PLUDyBU7LpUR3sOmjIJCdO-d6FswfN9t4QpLCmZC9RNQ9aX7YxC_S2buVwC3APy9x_YFnswH3iqaBulZ9DKx0I6SHP2PCroxxlq5DZSmlbvaH)

Kubeless comes as a native serverless framework on Kubernetes. This project comes from Bitnami. It extends from custom resource definition feature to be able to create custom resources on Kubernetes. Developers are able to understand what’s going on behind the scene and how it works quickly. When running, a in-cluster controller will be used to monitor resources and launch runtimes on-demand. Then, the function code will be injected into the runtimes dynamically.

[Project Page](https://kubeless.io/)  
[Source Code](https://github.com/kubeless/kubeless)  
[License](https://www.apache.org/licenses/LICENSE-2.0)  
Platform  
OSSPal Link

![](https://lh5.googleusercontent.com/8sy7qjm0ufK0HWIOtiz0KgDJaedmKwX4_9tFn7EuSG60qaClCeRZJYV1hryAl80WhsoFqqNFj0eGYrY1r5J9FCFBDdWs7Kxwa-ceXaSQN4C11x-gtBE0dTfRiMFLAlgEM2oLi7zt)

Funktion is also an open source project built on top of Kubernetes to provide serverless programming. It supports various kinds of trigger endpoint URLs, like network protocols, message systems, and databases. Originally Funktion is funded by Red Hat, but now Red Hat has stopped funding this project, and the bad news is that Funktion has no longer be maintained as well.

[Project Page](https://funktion.fabric8.io/)  
[Source Code](https://github.com/funktionio/funktion)  
[License](https://www.apache.org/licenses/LICENSE-2.0)  
Platform  
OSSPal Link

![](https://lh4.googleusercontent.com/AtxSObwicU7GalDVD36gtl91l3eZ03oogmOx69qRX48CVyp4OlAr8xKzVDsJzUGqqF7FUJgcVyjn21ECUHmRUgj4bMYu5nVsUJVgdGBIHnAIo8yriAyA3Stg-srbH_COSIq5ndEw)

OpenWhisk offers a programing model where developers can upload function event handlers to a cloud service and respond to various events. It is in the incubation stage in Apache Software Foundation. It can be used on top of Kubernetes cluster environment or use [Vagrant](http://vagrantup.com/) to run OpenWhisk. This project is under Apache incubator. As a result, OpenWhisk integrates lots of Apache projects in order to provide FaaS where it puts your code into a Docker container, and trigger them through a restful API. Nginx will be used to fielded the requests, and then turned into Kafka messages. CouchDB can be used to handle authentication and information management. IBM cloud function is based on OpenWhisk to provide FaaS platform.

![The internal flow of processing in OpenWhisk](https://lh5.googleusercontent.com/5mVdZy8JgQh6EfdeIRhbLdU_qMisaiv3N4JfRTGQd-mpiKc6eC_n4ZyRooEoYTZzlwSQBHYhn9ZAcLDtjLsYStPiFKcHDGNw-rRm4VNqQiwbtSrwZIy_j98DPwEU6jxx2SxdFljL)

[Project Page](https://openwhisk.apache.org/)  
[Source Code](https://github.com/apache/incubator-openwhisk)  
[License](https://www.apache.org/licenses/LICENSE-2.0)  
Platform  
OSSPal Link

#### **Competitive evaluation among these FLOSS tools/frameworks**

Here will do the competitive evaluation of different open source frameworks for serverless functions.

|  **** | **Fission** | **Kubeless** | **Funktion** | **OpenWhisk** |
| :--- | :--- | :--- | :--- | :--- |
| **HTTP** | **Y**ES | YES | YES | YES |
| **Web UI** | YES | YES | NO | NO |
| **Message Queue** | NATS, Azure Queue Storage | NATS, KAFKA | KAFKA | KAFKA, IBM Message Hub |
| **Language** | php,python,nodejs,go,ruby | php,python,nodejs,go,ruby | nodejs, python, ruby | js,swift,python,php,java,go |
| **Maintained** | YES | YES | NO | YES |
| **Maintainer** | Platform9 | Bitnami | Red Hat | IBM |
| **License** | Apache 2.0 | Apache 2.0 | Apache 2.0 | Apache 2.0 |

Kubeless has the kubeless-ui where developers can edit and deploy functions on the web console, which is similar to AWS Lambda. Fission also has the developer console, but it is not quite friendly as Kubeless. However, Fission has quite a lot more features than Kubeless, like logging and benchmark. Funktion recommend you to use Fabric8 to assist developers to write functions and deploy them.

Fission-workflow is another important feature for the production where functions can be completed with a specific order in a chain way, which is similar to AWS step functions. But Kubeless does not has this feature.  
****

![The Fission-workflow example](https://docs.google.com/a/west.cmu.edu/drawings/d/s1jKFL7kSvOM5HEyoB2DbwQ/image?w=524&h=64&rev=99&ac=1&parent=1EUsG35X6sKJWvdjt7U5mYhX2NKF0AWytOH5c6mLz6O0)

Kubeless will create one pod for each function and scale them as needed, while Fission will reuse the existing runtimes using the pool management. In real situation, if one of your function crashed in an unexpected way, Kubeless will create a new pod for you, which may take some time to prepare the resource, while Fission will use another pod in the pools, so the down-time of your service can be minimized.

Using Openwhisk in IBM’s cloud platform is a little different to open sourced Openwhisk. IBM already integrates it nicely and provides simple interface that allows you to write and run you code on the cloud platform, but it might take some time and encounters roadblock when you try to build your cloud service on your own.

To sum, Fission has rich features as well as web-based user interfaces and quite fast in terms of cold-start time, and it reuse the existing resources via pool management. But the support of Kafka is still on the construction. Kubeless has user friendly interfaces, support Python 2.7 natively. But it might incur using a lot of resources in production, and might have more down-time if some of your function crashed. Funktion is now not maintained, which would be a major disadvantage of this project. Openwhisk integrates with Apache projects very well. But it might take some time to build up your cloud service on your own in terms of configuration.

#### **References**

[\[1\] “Serverless Computing”, WikiPedia](https://en.wikipedia.org/wiki/Serverless_computing)  
[\[2\] “What is serverless architecture?”, marutitech](https://www.marutitech.com/serverless-architecture-business-computing/)  
[\[3\] Peter Wayner, "Open source serverless: Fission, Fn, Kubeless, and OpenWhisk", InfoWorl](https://www.infoworld.com/article/3279781/application-development/open-source-serverless-fission-fn-kubeless-and-openwhisk.html?nsdr=true)  
[\[4\] Nate Fonseka, “Kubeless vs Fission: The Kubernetes Serverless match up”, Medium](https://medium.com/@natefonseka/kubeless-vs-fission-the-kubernetes-serverless-match-up-41f66611f54d)  
[\[5\] Stephen Watts, "SaaS vs PaaS vs IaaS: What’s The Difference and How To Choose", bmc](https://www.bmc.com/blogs/saas-vs-paas-vs-iaas-whats-the-difference-and-how-to-choose/)  
[\[6\] Kash Kashyap, "3 simple use cases for leveraging serverless or FaaS “Functions as a Service” in your enterprise.", Mediu](https://medium.com/devopslinks/3-simple-use-cases-for-leveraging-serverless-or-faas-functions-as-a-service-in-your-enterprise-409d431b7552)  
[\[7\] Nilesh Suryavanshi, "What are Cloud Computing Services \[IaaS, CaaS, PaaS, FaaS, SaaS\]", Medium](https://medium.com/@nnilesh7756/what-are-cloud-computing-services-iaas-caas-paas-faas-saas-ac0f6022d36e)

  
  

