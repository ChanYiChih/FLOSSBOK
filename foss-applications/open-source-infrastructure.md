# Open Source Infrastructure

## Open Source Infrastructure

Open source infrastructure is generally defined as a group of free, open source tools used to support the daily running and maintenance of software. This includes basic network communication, the operating system, and several security tools. Open source infrastructure follows the same principle as open source software: “Given enough eyeballs, all bugs are shallow.” In other words, with enough people working on open source projects, a problem will be identified quickly and a fix will be obvious to someone. Therefore, the following are hallmarks of open source tools: configurations are shared openly in a source code repo; conduct planning and decision-making are transparent; follow the open source way to build infra community and apply four freedoms \(freedom to run the program, freedom to study how the program works, freedom to redistribute, freedom to distribute copies of your modified versions to others\) to infra details so the quality can be improved as more users submit their ideas and fixes. Open source projects have their origins in the infrastructure dimension. Prominent projects such as Apache HTTP server, the Nagios monitoring tool, and the Linux operating system are becoming more popular and well known today. More detailed information about these open source projects follows:

### HTTP Accelerator

HTTP accelerators, also called “reverse proxies,” are implemented on the side of Internet servers. They have different uses including security, load balancing, SSL acceleration, compression, and cache. It is this last point, in particular, that we evaluate in this section. Internet users “pass” through proxy reverses to access applications from internal servers. Advanced caching policies can unload Web application servers regardless of the language used. Some HTTP accelerators manage the cache fragment, including supporting the ESI standard.

### Cloud Computing

One of the key ideas behind the somewhat vague concept of cloud computing is the abstraction of an application’s platform at various levels. This can include IaaS \(Infrastructure as a Service\), in particular but also PaaS \(Platform as a Service\) and SaaS \(Software as a Service\).

Naturally, virtualization is crucial to setting up IaaS. However, it requires making virtual machines available in a completely automated manner. Monitoring resource use for billing purposes is part of the cloud-computing business model and thus should be an integral part of any IaaS solution. The product should also handle the automatic configuration of a  permanent storage space for VMs, as well as providing for their network connectivity. For organizations wishing to build their own IaaS, open source solutions like OpenStack are now available and make it possible to industrialize virtualization.

### Remote Computer Control

Remote computer control solutions are becoming increasingly available, and their technology has advanced impressively in recent years. These tools were initially created to meet user support and assistance needs. They can be either localized or spread across some or all of a company’s client workstations, as needed. They are used to respond to the different issues encountered by companies, including shared views of computers and file transfers. The open source range in this category includes tools like TightVNC and OpenSSH. The latter is the favorite among systems administrators in the world of UNIX servers.

### VPN

A virtual private network \(VPN\) extends a private network across a public network and enables users to send and receive data across shared or public networks as if their computing devices were connected directly to the private network. Applications running across the VPN may thereby benefit from the functionality, security, and management of the private network.

### Linux & BSD Operating System

FreeBSD is a free and open source Unix-like operating system descended from via Berkeley Software Distribution \(BSD\). Although for legal reasons FreeBSD cannot use the Unix trademark, it is a direct descendant of BSD, which was historically called “BSD Unix” or “Berkeley Unix.” The first version of FreeBSD was released in 1993, and today FreeBSD is the most widely used open source BSD distribution, accounting for more than three-quarters of all installed systems running open source BSD derivatives.

### Free and Open Source Resources

There are many resources available for starting to learn about open source infrastructure, open source tools, and projects that lay the foundation for a sound infrastructure that is capable of hosting the best applications under optimal conditions.

### Books

* [The Open–source PKI Book \(2000\)](http://ospkibook.sourceforge.net/docs/OSPKI-2.4.7/OSPKI-html/ospki-book.htm) 
* [Cooking Infrastructure by Chef \(2014\)](http://chef.leopard.in.ua/)

### Articles

* [The Open Sourcing of Infrastructure \| Opensource.com](https://opensource.com/article/17/8/open-sourcing-infrastructure) 
* [Open sourcing the infrastructure of a project \| Opensource.com ](https://opensource.com/article/17/3/growth-open-source-project-infrastructures)
* [Infrastructure / Open Source Guide ](http://www.open-source-guide.com/en/Solutions/Infrastructure)
* [How to set up an all open-source IT infrastructure from scratch](https://www.networkworld.com/article/3217713/open-source-tools/how-to-set-up-an-all-open-source-it-infrastructure-from-scratch.html)

### Online Courses

* [Introduction to Cloud Infrastructure Technologies](https://www.edx.org/course/introduction-cloud-infrastructure-linuxfoundationx-lfs151-x)

## Proprietary Resources

### Books

* [Cloud Native Infrastructure \(2017\) ](https://www.amazon.com/Cloud-Native-Infrastructure-Applications-Environment/dp/1491984309)
* [Practical Linux Infrastructure \(2014\) ](https://www.amazon.com/Practical-Linux-Infrastructure-Syed-Ali/dp/148420512X)
* [Open Source Security Tools \(2004\)](https://www.amazon.com/Open-Source-Security-Tools-Applications/dp/0321194438)

### Video Training

* [The Open Sourcing of Infrastructure ](https://www.youtube.com/watch?v=Ux7DZ38aGIc)
* [Open Source Infrastructure – Jose Gonzalez @savant ](https://www.youtube.com/watch?v=264ho9xqeJU)
* [“Eucalyptus: An Open Source Infrastructure for Cloud Computing” – Rich Wolski](https://www.usenix.org/conference/lisa-09/eucalyptus-open-source-infrastructure-cloud-computing)

## Major Open Source Infrastructure Tools and Solutions

### HTTP Accelerator

#### Varnish – HTTP accelerator \[1\]

Varnish Cache is a web application accelerator. It’s installed in front of any web server that speaks HTTP and configured to cache the contents. It acts as a web application accelerator, focusing on optimizing caching and compression. It is really fast and used by high-traffic FOSS Infrastructure 14 websites such as Wikipedia, Facebook, Twitter, and others. Varnish claims to deliver 20 Gbps on regular off-the-shelf hardware. 

* [Project Page ](https://varnish-cache.org/)
* [Source Code ](https://github.com/varnishcache/varnish-cache)
* License: [Two-clause BSD license](https://en.wikipedia.org/wiki/BSD_licenses)
* Platform: BSD, Linux, Unix 
* OSSpal Link

#### HAProxy – Load balancer and proxy server accelerator \[2\]

HAProxy is an open source software-based load balancing, SSL offloading and performance optimization, compression, and general web-routing software. HAProxy is used by some high-profile websites including GitHub and Reddit; it’s also used in the OpsWorks product from Amazon Web Services. I have seen a healthy system achieve between 15,000 and 30,000 hits per second, with no trouble saturating a 2-Gbit/sec connection. HAProxy claims to deliver 10GbE load balancing or higher. 

* [Project Page ](http://www.haproxy.org/)
* [Source Code ](https://github.com/haproxy/haproxy)
* License: [GPL v2 ](https://en.wikipedia.org/wiki/GNU_General_Public_License)
* Platform: BSD, Linux, Unix, Aix, Solaris 
* OSSpal Link





