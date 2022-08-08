# Class 16 - What is Serverless

* Serverless - A cloud application development and execution model where developers can build and run code without managing servers or paying for idle cloud infrastructure
  * Developers focus on writing code then deploy it to containers
  * These containers are managed by a cloud service provider
  * Cloud providers spin up and provisions the required resources to execute the code and then spins them back down - "scaling to zero"

## Serverless does not mean 'no servers'
* Serverless describes the developers experience, not the entire experience

## Serverless is more than just FaaS (Function-as-a-service)
* FaaS - cloud computing service that enables devs to run code in response to specific events, without specifying or managing the infrastucture
* Serverless databases and storage
  * Serverless demands getting away from capacity, connection, and query limits of databases and scaling them linearly

## Serverless vs PaaS, containers and VMs
* Provisioning time:
  * Measured in milliseconds for serverless
  * Measured in minutes to hours for other models
* Administrative burden:
  * No burden for serverless
  * Light to medium to heavy for Paas, containers and VMs
* Maintenance:
  * Serverless are managed 100% by the provider
  * Same is true for PaaS
  * Containers and VMs require significant maintenance - updating/managing OS, container images, connections, ect
* Scaling:
  * Auto-scaling is instant for serverless
  * Automatic by slow scaling that requires fine tuning of auto-scaling rules and no scale to zero
* Capacity planning:
  * None needed for serverless
  * Others require a mix of automatic scalability and some capacity planning
* Statelessness:
  * Inherent for serverless, state is maintained by external provider
  * Otheres can leverage HTTP, keep an on socket connnection for long periods and store state in memory
* High Availability (HA) and Disaster Recovery (DR):
  * Both are inherent in serverless with no extra effort or cost
  * Other models require extra cost/management effort
* Resource Utilization:
  * Serverless is 100% efficient because there is no idle capacity
  * All other models involve some form of idle capacity
* Billing Granularity and Savings:
  * Serverless is metered in units of 100 milliseconds
  * Others are metered by the hour or minute

## Serverless, Kubernetes and Knative
* Kubernetes
  * Open source container platform which automates deployment, management, and scaling of containers
  * Cannot run serverless apps without specialized software that integrates Kubernetes with cloud providers platforms
* Knative
  * Provides serverless framework for Kubernetes
  * Open osurce extension to Kubernetes

* Knative is transparent to devs - they build a container as usual using Kubernetes and Knative does the rest

## Pros and Cons of Serverless
* Pros
  * Improved Developer Productivity
    * Devs can focus on code and not managing infrastructure
  * Pay for execution only
    * Meter starts when request is made and ends after execution
  * Develop in any language
    * Polygot environment enables any language or framework
  * Streamlined development/DevOps cycles
  * Cost-effective performance
  * Usage Visibility
* Cons
  * Unacceptable latency for certain applications
    * Because of scaling from zero you cannot get instant execution
    * Think financial institutions
  * Higher costs for stable or predictable workloads
  * Monitoring and debugging issues
  * Vendor lock-in
