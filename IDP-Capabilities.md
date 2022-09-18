Copyright 2022 Adobe
All Rights Reserved.

NOTICE: Adobe permits you to use, modify, and distribute this file in
accordance with the terms of the Adobe license agreement accompanying
it.


# IDP Capabilities

![IDP Capabilities](./images/IDP-Capabilities.png?raw=true)

Adobe Internal Developer Platform (IDP) aims to make the lives of internal developers easier by providing a seamless experience for the entire development lifecycle, from concept → code → cloud → customers, with production readiness built in.

## Discover and Create

Discover and Create capabilities cover the initial part of the development lifecycle, including onboaring, training, bootstraping, local development etc. 


### Architecture Guidance & Tools

Guide developers as they design their project with architecture and tooling. This includes:

* Design Patterns and best practices
* Templates and Bootstrapping solutions
* Production readiness guidance
* Reference apps, snippets, libraries and images


### Documentation Training & Certification

Help developers understand how to leverage the platform to the maximun, in a self-service manner. 

Facilitate a community around the platofm, where individuals from different service teams become SMEs on the platform and can help their team achieve their goals without having to wait for the platform team for information or help. This includes:

* Platform usage guides
* Training docs and videos
* Community brown-bags and office hours

### Developer Portal & Dashboards

One-stop-shop for everything the developers need to onboard, configure and observe their services. This includes, in high level terms:

* Ability to visualize the desire state of the system and service
* Ability to view the actual state of the system and service
* Helm in editing the desired state in its source-of-truth location (eg GitHub) 


### Automated Support & Search

Provide developers with a self-serve way to find information about the platform and its features, get responses to questions and automated help for problems. This includes:

* Tools to search all available docs, guides, examples etc, in an intuitive and easy way


### Version Control & IDE Tools

Make development, including local development and testing, easy and efficient. This includes:

* Version control tools
* IDE plugins 
* Local dev and testing environments 
* Ephemeral cloud dev and testing environments 


### Service Generation

Automated and templatized way to bootstrap and configure a service/application from scratch, which:

* Are tested and hardened
* Include best practices 
* Include security and compliance built-in


### Service Management & Discovery

A service directory that can be searched, including:

* Available services and their metadata 
* Their API spec 

---

## Integrate and Deploy

Integration and Deploy capabilities cover deployment, integration of distributed systems, configuration of resources etc.

### Environment Management

Ability to easily create, configure and manage service/app environments. Includes:

* Initial onboarding of a service with a set of environments
* Easily adding a new environment/region, or removing an old one
* Creating and removing Ephemeral environments for development, testing or experimentation
* Easily manage environment-specific configurations and resources


### Configuration Management

Developers should manage application configuration in a scalable and reliable way, similarly to how we manage and version source code. This includes:

* Manage the service/application 
* Manage cluster resources
* Manage other (non-cluster) cloud resources


### Infrastructure Provisioning & Orchestration

Ability to provision and configure cloud resources and other infrastructure for the service/app leveraging GitOps. This includes:

* Defining all required resources as code (including clusters), as part of the service/app configuration definitions
* Ability to automatically associate resources credentials and configuration that is needed by the service/app, on a per-environment basis
* Just-in-time provisioning of all required resources as part of the application/app provisioning


### Delivery/Deployment Management

Ability to easily manage the CI/CD for the service/app, including:

* Defining the following as code:
    * Service/app delivery/deployment logic, including any triggers and workflows
    * Progressive delivery rules 
    * Desired notifications
    * Tests and conditional environment promotions
* Observability of current state and history
* Debugging tools
* Ability to repeat past deployments reliably


### API Management

Ability to easily onboard and manage the API configuration of the service as code, in a self-service manner, including:

* API Authentication and Authorization validations
* API routing and traffic managemenr (like throttling, routing configs etc)


### Secrets Management

Ability to easily onboard and manage secrets required by the service/app and supporting resources, including:

* Abitlity to associate environment-specific instances of the service/app with credentials and other secrets of resources for that environment
* Automatic integration of the secrets management system with the deployment/delivery system

### Workflow Orchestration

Ability to define and configure workflows as code, for various use-cases including:

* CI/CD 
* ML 
* Data processing

### Artifact Management

Ability to define and manage as code any artifacts required for the service/app deployment/delivery. This includes:

* Image repositories
* Generic repositories 
* Generic users/accounts

---

## Operate and Improve

Operate and Improve capabilities include management of the service/app at runtime, observability, monitoring etc. 


### Policy Management

Include management and enforement of business and operational policies on running apps/services.


### Cluster Releases & Management

Ability to manage the cluster fleet as code, with best practices and continuous deployment.

### Roles & Permissions

Management of RBAC, Authentication and Authorization of users and tools to the cloud resources and systems.

### Security

Management and enforcement of security policies and automatic validations and checks.

### K8s Clusters & Components

Management of the Kubernetes cluster fleet and components, including:

* RBAC
* Efficiency tooling

### Cloud Compliance, Governance

Management and enforcement of cloud policies and governance.

### Network engineering

Management of traffic and connectovity within and between the cluster fleet, corp network, and public internet. 


### Cloud Providers and Private Cloud

* Management of cloud provider accounts and resources.

### Diagnostics & Insights

Tools and dashboards to allow for diagnostics debugging of the running system to reduce MTTR (mean time to resolution)

### Observability

Ability to observe the running systems and understand their state and status.

### Monitoring

Ability to define as code dashboards and alerts to help with discovery and resolution of runtime issues.

### Reliability Engineering

### Incident Management

Ability to efficiently alert and notify engineers when business-impacting incidents/outages occure, as well as the tools for managing those incidents.

### Efficiency

Tooling for automatically improving the efficiency of the cloud resources, to minimize cost while not compromizing reliability.

### Quality Assurance & Testing Infra

Toos and frameworks for helping engineers validate the quality of the services/apps. Includes:

* Functional testing
* Chaos testing
* Load testing 
* Performance testing



