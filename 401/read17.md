# Read: Class 17 : AWS: S3 and Lambda

---

## Review, Research, and Discussion

- **Describe “The Cloud”**

  The cloud refers to software and services (computer) that run on the Internet, instead of locally on your computer. cloud computing is the delivery of computing services—including servers, storage, databases, networking, software, analytics, and intelligence—over the Internet (“the cloud”) to offer faster innovation, flexible resources, and economies of scale.

- **What is a container (as it relates to computers and servers)?**

  A container is a standard unit of software that packages up code and all its dependencies , Containers are a form of operating system virtualization. A single container might be used to run anything from a small microservice or software process to a larger application.

- **What is auto-scaling?**

  a method used in cloud computing that dynamically adjusts the amount of computational resources in a server farm - typically measured by the number of active servers - automatically based on the load on the farm (based on defined situations such as traffic ir utilization levels)

- **What is bandwidth?**

  bandwidth is the maximum rate of data transfer across a given path.

- **How do cloud providers compute service costs?**

  They start by calculating costs for network hardware, network infrastructure maintenance, and labor.

  > **_Networking costs_**: The vendor decides how much it must spend to maintain the network. Consequently, the provider estimates the costs for the hardware, network setup, labor and maintenance.  
  > **_Computing costs_**: The provider calculates the costs for CPUs -- client organizations will have their own individual requirements when it comes to using CPUs. Costs also include licensing fees, depending on the operating system an organization is running. The provider calculates the costs of buying hardware for every gigabyte of virtual RAM that a company uses.  
  > **_Storage costs_**: The vendor calculates how much it will cost to operate a company's storage hardware or what it will cost to buy new hardware to meet the storage needs of the enterprise.

---

### Document the following Vocabulary Terms

- **Server Instances** A server instance is a collection of SQL Server databases which are run by a solitary SQL Server service or instance. The details of each server instance can be viewed on the service console which can be web-based or command-line based.

- **Containers** A container is a standard unit of software that packages up code and all its dependencies , Containers are a form of operating system virtualization. A single container might be used to run anything from a small microservice or software process to a larger application.

- **Cloud Services** Cloud computing is the on-demand availability of computer system resources, especially data storage and computing power, without direct active management by the user. Large clouds often have functions distributed over multiple locations, each location being a data center

- **Cloud Architecture** Cloud architecture is the way technology components combine to build a cloud, in which resources are pooled through virtualization technology and shared across a network. The components of a cloud architecture include: A front-end platform (the client or device used to access the cloud) , A back-end platform (servers and storage) , A cloud-based delivery model , A network . Together, these technologies create a cloud computing architecture on which applications can run, providing end-users with the ability to leverage the power of cloud resources.

- **AWS** AWS (Amazon Web Services) is a comprehensive, evolving cloud computing platform provided by Amazon that includes a mixture of infrastructure as a service (IaaS), platform as a service (PaaS) and packaged software as a service (SaaS) offerings.

---

## Preview

Which 3 things had you heard about previously and now have better clarity on?

--

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

--

What are you most excited about trying to implement or see how it works?

--

---

> **_Content Delivery Network (CDN) _** : is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos. Employing a CDN doesn’t only speed up the delivery of Internet content, it helps protect your website against certain forms of cyber attacks, It protects against these threats because CDNs allow for the handling of more traffic and withstanding hardware failure better than many origin servers.

> **_ AWS Lambda _**: a serverless compute service that lets you run code without provisioning or managing servers, creating workload-aware cluster scaling logic, maintaining event integrations, or managing runtimes. With Lambda, you can run code for virtually any type of application or backend service - all with zero administration.

common use cases :

- individual tasks run for a short time
- each task is generally self-contained
- there is a large difference between the lowest and highest levels in the workload of the application.

Benefits :

- Pay per use
- Fully managed infrastructure
- Automatic scaling.
- Tight integration with other AWS products

> **_Amazon Simple Storage Service (Amazon S3) _** : an object storage service that offers industry-leading scalability, data availability, security, and performance. This means customers of all sizes and industries can use it to store and protect any amount of data for a range of use cases, such as data lakes, websites, mobile applications, backup and restore, archive, enterprise applications, IoT devices, and big data analytics
