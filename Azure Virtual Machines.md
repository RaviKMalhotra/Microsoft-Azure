 ![image](https://github.com/user-attachments/assets/da5df687-7c71-492f-ac84-3f148cb0440e)
 
| Personal            | Details                                     | 
|---------------------|---------------------------------------------|
| 👤✍️ Author        | Ravi K Malhotra -                           |  
| 🌐 Website          | www.ravikmalhotra.com                       | 
| 🚀 Linkedin Profile | https://www.linkedin.com/in/ravikmalhotra/  | 
| 🐱 Github profile   | https://github.com/RaviKMalhotra            | 
| 📜Topic             | Overview of Azure Virtual Machines (🖥️)      |

# Overview of Azure Cloud Compute Services
💡 🚀 ♾️ 🛡️  ⬣  🟣   🔵  🟢  🟡  🔴   🔴   🔺 

## 01. Virtual Machines Documentation link - https://learn.microsoft.com/en-us/azure/virtual-machines/
## 02. Compare virtual-machine based compute products - https://learn.microsoft.com/en-us/azure/virtual-machines/compare-compute-products?tabs=prodcompcost
## 03. Learn how to create a linux VM
## 04. Learn how to create a Windows VM
## 05. Learn how to create a Virtual Machine Scale Set
#



# Lab: Create a Linux VM
# Lab: Create a Windows VM
# Lab: Create a Virtual Machine Scale Set
# Lab: Create a VM - Static Public IP
Create a VM - Static Private IP
Create a VM - Multiple IPs
Create a VM - Accelerated Networking
Use Multiple NICs
 
- Compute services are the most critical and highly used components in any cloud platform.
- Compute instances are also referred as workloads, as you can host any website or any custom application on top of a compute instances.
- Compute services in GCP are offered as both IaaS and PaaS types.
- GCP compute engine is a form of IaaS cloud computing, whereas App engine is a form of PaaS cloud computing.
- Compute instance, simply means a virtual machine in Microsoft Azure Cloud and EC2 instance in AWS cloud.
- GCP offers a wide range of compute services. Here is a list
    - GCP App Engine
    - GCP Compute Engine
    - Google Kubernetes Engine (GKE) (Managed Kubernetes)
    - Cloud Functions (FaaS - Even Drien Serverless)
    - Cloud Run (Serverless Containers)
    - Bare Metal Solution (Dedicated Hardware for Specialized Workloads)
    - Anthos (Hybrid and Multi-Cloud Management)
      
## 1. GCP App Engine

- Google App Engine is one of the earliest cloud computing services from Google.
- launched in 2008 as a pioneering **Platform as a Service (PaaS)**.
- It allows developers to build, deploy, and scale applications without worrying about managing the entire infrastructure.
- With automatic scaling, built-in load balancing, and support for multiple programming languages, App Engine enables businesses to focus solely on writing code while Google takes care of hosting and operations.
- Whether you are building a simple web app or a complex enterprise application, App Engine provides a seamless, fully managed environment to deploy applications effortlessly."
- Primary Use Cases: Web apps, APIs, and backend services.

### These are the Key Features of an GCP App Engine:

✅ Fully managed runtime environments (Python, Java, Go, Node.js, PHP, Ruby, etc.).

✅ Automatic scaling & load balancing.

✅ Integrated monitoring with Cloud Logging & Trace.

✅ Traffic Splitting (A/B testing for different versions).

✅ Built-in security & compliance.

## 2. GCP Compute Engine

- "When it comes to raw compute power and flexibility, Google Compute Engine stands as the backbone of Google Cloud’s infrastructure services.
- Launched in 2012, it provides highly customizable virtual machines (VMs) that can run various workloads, from web applications to high-performance computing.
- Compute Engine offers full control over VM configurations, allowing businesses to choose the right balance of CPU, memory, and disk storage to match their needs.
- With built-in security, live migration, and automatic scaling, it ensures that workloads remain performant, reliable, and cost-efficient."
- Compute Engine is an Infrastructure as a Service (IaaS) offering that provides scalable virtual machines (VMs) on Google's infrastructure.
- It supports both Windows and Linux operating systems.
- you can create compute engine using the GCP console, and the CLI mode.
- It offers various machine types to suit different workloads.
- As this being an IaaS offerings, users or consumers have full control over VM configurations, including CPU, memory and storage options.
- Primary use cases of Compute Engine: Web hosting, databases, big data processing, and enterprise applications.
 
### These are the Key Features of GCP Compute Engine:
✅ Fully customizable VMs (CPU, RAM, disk, and GPU).

✅ Preemptible and Spot VMs (cost-saving for non-critical workloads).

✅ Live Migration (keeps VMs running during maintenance).

✅ Autoscaling & Load Balancing (optimizes performance).

✅ Confidential Computing (encrypts data in use).


## 3. Google Kubernetes Engine (GKE) (Managed Kubernetes)

- "Managing containers at scale can be complex, but Google Kubernetes Engine (GKE) simplifies this process by providing a fully managed Kubernetes environment.
- Since its launch in 2015, GKE has enabled organizations to **deploy, manage, and scale containerized applications seamlessly.**
- Built on Google’s expertise with Kubernetes—the open-source container **orchestration platform** that originated at Google—GKE provides auto-scaling, security, and multi-cluster support.
- **Whether running workloads on Google Cloud or in hybrid/multi-cloud environments with Anthos, GKE offers a powerful and flexible container management solution."**
- - GKE is a managed Kubernetes service that simplifies deploying, managing, and scaling containerized applications using Google's infrastructure. 
- It offers automated operations, integrated security, and enterprise-grade support.
- Primary use cases of Google Kubernetes Engine: Microservices, hybrid/multi-cloud applictions, and container orchestration.

### Key Features of Google Kubernetes Engine (GKE):

✅ Auto-scaling (automatically adjusts compute resources).

✅ GKE Autopilot (fully managed mode where Google handles cluster operations).

✅ Multi-cluster & Multi-region support.

✅ Built-in security features (IAM, encryption, and vulnerability scanning).

✅ Hybrid and Multi-cloud Support (via Anthos).

## 4. Cloud Functions (FaaS - Even Drien Serverless)

- FaaS stands for Functions-as-a-service.
- "Cloud Functions revolutionizes **application development** by providing a **serverless**, **event-driven computing model**.
- Introduced in 2017, this Function as a Service (FaaS) offering **lets developers execut**e **lightweight functions in response to triggers from various Google Cloud services**, such as Cloud Storage, Pub/Sub, and Firestore.
- Since it automatically scales and charges only for execution time, it eliminates the need for provisioning or managing servers, making it an ideal solution for real-time data processing, automation, and microservices-based architectures."
- A Function as a Service (FaaS) runs event-driven code without managing servers.
- Primary Use Cases: Real-time data processing, IoT, API automation, and event-driven workloads.
- 
### Key Features of Google Functions (FaaS - Event Drive serverless)

✅ Fully serverless (only pay for execution time).

✅ Triggers from GCP services (Cloud Storage, Pub/Sub, Firestore, etc.).

✅ Autoscaling from 0 to N requests.

✅ Built-in security & monitoring.

✅ Supports multiple runtimes (Node.js, Python, Go, Java, .NET, Ruby, PHP).


## 5. Cloud Run (Serverless Containers)

- "Bridging the gap between serverless computing and containerization, **Cloud Run** provides a fully managed platform for running stateless, containerized applications.
- Launched in 2019, **it enables businesses to deploy any application packaged as a container without worrying about infrastructure management.**
- **Cloud Run automatically scales based on demand and even scales down to zero when idle, ensuring cost efficiency.**
- Its support for multiple programming languages, seamless integration with Google Cloud services, and built-in security features make it an attractive choice for modern application development."
**- Google Cloud Run is a serverless compute platform for running stateless containerized applications.**
Primary Use Cases: Deploying microservices, APIs, and web applications.

## Key Features of Google Cloud Run 

✅ Deploy any containerized app (supports Docker & OCI-compliant containers).

✅ Scales to zero when idle (cost savings).

✅ Fully managed or Anthos-managed (for hybrid/multi-cloud).

✅ Supports HTTP-based workloads & WebSockets.

✅ Integrated with GCP IAM & Cloud Logging.

## 6. Bare Metal Solution (Dedicated Hardware for Specialized Workloads)

- "Remember that Not all workloads are designed for virtualized environments", which is why Google Cloud introduced Bare Metal Solution in 2020.
- This offering provides dedicated physical servers for applications that require specialized hardware, such as Oracle databases and high-performance computing (HPC).
- Bare Metal Solution gives enterprises the flexibility to run these workloads close to Google Cloud services while maintaining compliance and performance requirements.
- With low-latency connections and full control over the hardware, it is an ideal choice for businesses with demanding compute needs.

### Key Features of Bare Metal Solutions
✅ No virtualization overhead (bare metal performance).

✅ Low-latency connectivity to Google Cloud services.

✅ Supports custom licensing requirements.

✅ Enterprise-grade security & compliance.


## 7. Anthos (Hybrid and Multi-Cloud Management)

- "As cloud adoption grows, many businesses operate in hybrid or multi-cloud environments, **requiring a unified management platform**.
**- Anthos, introduced in 2019, addresses this need by allowing organizations to manage applications consistently across Google Cloud, on-premises data centers, and even other cloud providers like AWS and Azure.**
- Google Anthos is Built on Kubernetes and service mesh technologies.
- Google Anthos provides a secure and scalable framework for modernizing applications without being locked into a single cloud provider.
- It empowers businesses **to deploy workloads anywhere** while maintaining visibility, security, and compliance across environments."

### Key Features of Anthos Solutions

✅ Run workloads anywhere (on-prem, AWS, Azure).

✅ Uses GKE for Kubernetes management.

✅ Anthos Config Management (enforces policies across environments).

✅ Service Mesh for microservices security & observability.

### Here is a tabular representation of each of GCP Compute Services:

| Service                       | Type                   | Best For                     | Key Feature   |
|-------------------------------|------------------------|------------------------------|---------------|
| Compute Engine                | IaaS                   | Virtual Machines             | Data          |
| GKE (Google Kubernetes Engine | Managed Kubernetes     | Containers & Microservices   | Data          |
| App Engine                    | PaaS                   | Web & Backend Apps           | Data          |
| Cloud Functions               | FaaS                   | Event-drive workloads        | Data          |
| Cloud Run                     | Serverless Containers  | stateless containerized apps | Data          |
| Bare Metal Solutions          | Dedicated Hardware     | Specialized workloads        | Data          |
| Anthos                        | Hybrid/Multi-Cloud     | Hybrid & Multi-Cloud Apps    | Data          |


## Conclusion & Final Thoughts


  ### Ravi K Malhotra


