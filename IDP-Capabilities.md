Copyright 2022 Adobe
All Rights Reserved.

NOTICE: Adobe permits you to use, modify, and distribute this file in
accordance with the terms of the Adobe license agreement accompanying
it.


# IDP Overview

![IDP Capabilities](./images/IDP-Capabilities.png?raw=true)

Adobe Internal Developer Platform (IDP) aims to make the lives of internal developers easier by providing a seamless experience for the entire development lifecycle, from concept → code → cloud → customers, with production readiness built in.

This diagram outlines the common capabilities that an IDP has, which are used by developers during the service/app development lifecycle.  

In [a 2022 Gartner report](https://www.gartner.com/en/documents/4010078), these IDP capabilities are categorized into the following three development lifecycle phases:

* Discover and Create
* Integrate and Deploy
* Operate and Improve

We'll now expand a bit on each of these phases and capabilities.

## Discover and Create

Discover and Create capabilities cover the initial part of the development lifecycle, including onboarding, training, bootstraping, local development etc. 


### Architecture Guidance & Tools

Guide developers as they design their project with architecture and tooling. This includes:

* Design Patterns and best practices
* Templates and Bootstrapping solutions
* Production readiness guidance
* Reference apps, snippets, libraries and images

### Documentation Training & Certification

Help developers understand how to leverage the platform to the maximun, in a self-service manner. 

Facilitate a community around the platform, where individuals from different service teams become SMEs on the platform and can help their team achieve their goals without having to wait for the platform team for information or help. This includes:

* Platform usage guides
* Training docs and videos
* Community brown-bags and office hours

### Developer Portal & Dashboards

One-stop-shop for everything the developers need to onboard, configure and observe their services. This includes, in high level terms:

* Ability to visualize the desired state of the system and service
* Ability to view the actual state of the system and service
* Help in editing the desired state in its source-of-truth location (eg GitHub) 

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

Management and enforcement of business, operational, and other policies on running apps/services and resources. This includes:

* Restricting resource configurations to allowed values
* Enforcement of specific annotations/labels
* Enforcement of specific configurations on production environments

### Roles & Permissions

Management of RBAC, authentication and authorization of users and tools to the cloud resources and systems. Examples include:

* Managing K8s clusters access level based on roles, for example different access for service operators and cluster operators
* Defining RBAC permissions to perform deployments, updates to the configuration of the service/app and resources

### Security

Definition and enforcement of security policies and automatic validations and checks. This includes:

* Security reviews and approvals
* Scanning and checks for vulnerabilities 


### K8s Clusters & Components

Management of the Kubernetes cluster fleet and components as code, with best practices and continuous deployment, including:

* Framework for cluster components
* Clusters release management


### Cloud Compliance, Governance

Management and enforcement of business policies and governance. This includes:

* Framework for implementing measures for compliance with business policies 
* Framework for adhering to governance rules and regulations

### Network engineering

Management of traffic and network connectivity. This includes:

* Network policies (ingress and egress) within and between the cluster fleet, cloud resources, corp network, and public internet
* Management of network performance and latency
* Network throughput and reliability

### Cloud Providers and Private Cloud

Management of cloud provider and Data Center accounts and resources. This includes:

* Tooling (including CLI/UX) for accounts management
* Management of policies for resources inside the cloud provider accounts and in the data centers

### Observability

Ability to generate all the needed data in order observe the expected, unexpected and unanticipated status of the running systems. This includes:

* Logging and events
* Tracing
* Metrics

### Monitoring

Ability to use metrics to define dashboards and alerts as code to help with discovery and resolution of expected runtime issues. This includes:

* Dashboards
* Alerts

### Diagnostics & Insights

Tools and dashboards that use observability and monitoring data to diagnose issues and debug running systems in order to reduce MTTR (mean time to resolution). This includes:

* Automated detection of issues
* Automated root cause analysis
* Tools to help developers diagnose and analyse issues
* Automated remediation for self recovery of systems


### Incident Management

Ability to efficiently alert and notify engineers when business-impacting incidents/outages occure, as well as providing tools for managing those incidents. This includes:

* Incident management dashboards
* Incident management virtual situation rooms
* Tooling for alerting and creating situation rooms

### Efficiency

Tooling for automatically improving the efficiency of cloud resources usage, to minimize cost without compromizing reliability, and manage charge-back for multi-tenant clusters. This includes:

* Dashboards for efficiency and cost reporting
* Tools for cost chargeback 
* Tools for auto adjust resource requests according to the actual usage
* Tools to auto recommend configs for services for better efficiency 

### Reliability, Quality Assurance & Testing Infra

Toos and frameworks for helping engineers validate the quality of the services/apps. Includes:

* Functional testing
* Chaos testing
* Load testing 
* Performance testing



