# DevOps

## Operating Systems

### [Ubuntu](http://ubuntu.com/)

Many Linux distributions are available, but Ubuntu is one the the most popular ones and has a fast learning curve. Its server version is commonly used as a basis for many services.

### [NixOS](https://nixos.org/) <Badges user="NixOS" repo="nixpkgs"/>

The [MSF](https://www.msf.org/) Operational Center of Brussels [configured NixOS](https://github.com/MSF-OCB/NixOS) to be deployed in lightweight [NUC](https://en.wikipedia.org/wiki/Next_Unit_of_Computing) local servers. It standardises the installation, maintenance and monitoring of a cluster of remote server that is kept at a state defined in a unique Git repository. It is orchestrated through secure SSH relays and does not require a reliable connectivity.

<!-- ## Networking and Security

### OpenSSL

### LetsEncrypt

### AES

### GnuPG -->

## Reverse Proxies

### [Traefik](https://traefik.io/) <Badges user="containous" repo="traefik" />

Traefik can be used as an HTTP reverse proxy and load balancer, and goes along with Docker and Docker swarm pretty well, as it supports annotations, meaning there is no need to change Traefik's configuration when endpoint services change, as service-specific rules are defined together with each Docker service.

### [Ngnix](https://www.nginx.com/) <Badges user="nginx" repo="nginx" />

Nginx is a web server that is often used for the distribution of static files, but also for its load balancer, reverse proxy and cache capabilities. It is usually chosen for its excellent performance, but its advanced configuration requires some learning time.

## [Docker](https://www.docker.com/) <Badges user="docker" repo="docker-ce" />

Docker allow to virtualize operating systems that dramatically ease the delivery of software into containers. Docker became a standard in the cloud computing industry, as it allows to deploy almost any software in almost any type of host machine, bare metal or cloud.

## Container Orchestration

### [Kubernetes](https://kubernetes.io/fr/) <Badges user="kubernetes" repo="kubernetes" />

Kubernetes is a portable, extensible, open-source platform for managing containerized workloads and services, that facilitates both declarative configuration and automation. It allows to run large cluster of servers in order to ensure high availability. It has a large, rapidly growing ecosystem. Kubernetes services, support, and tools are widely available. Google open-sourced the Kubernetes project in 2014.

### [Docker Swarm](https://docs.docker.com/engine/swarm/) <Badges user="docker" repo="swarm" />

Docker Swarm allows to create clusters of docker machines quite easily, in order to ensure high availability of services.

### [Knative](https://cloud.google.com/knative/) <Badges user="knative" repo="serving"/>

Knative is a serverless solution that run on a Kubernetes cluster. It allows to optimize operational costs, and to facilitate integration and delivery processes through GitOps pipelines.

## CI/CD

Continuous Integration (CI) is a process to automatically build a software from different packages, source code and configuration into one single deliverable package, while testing its consistency in performing automated tests. Continuous delivery (CD) allows to automatically install this software in production, so the end user can have access to its last version. CI/CD platforms allow to reduce the time between the development of a feature, its validation and its access by the end user. They allow to work in very short iterations and to embrace agile project management methodologies. They also enable to correct bugs on time.

Numerous benchmarks of CI/CD platforms are available on the Internet. The following solutions worth a try and all work well together with GitHub in order to trigger pipelines:

### [Jenkins](https://jenkins.io/) <Badges user="jenkinsci" repo="jenkins" />

Jenkins is one of the oldest CI/CD platforms. I can be installed on a server, and hundreds of plugins are available. However the quality of those plugins may vary, and the design of elaborated pipelines may result in unnecessary complexity.

### [Drone.io](https://drone.io/) <Badges user="drone" repo="drone" />

Drone CI/CD is entirely built on Docker containers. It allows to quickly build pipelines and steps either from built-in containers, or to create its own plugins. The building platform can be easily run on premises, and the free-tier cloud solution is enough for developing simple software.

### [JenkinsX]() <Badges user="jenkins-x" repo="jx" />

JenkinsX is a CI/CD platform that runs on a Kubernetes cluster. It allows to define pipelines that goes from code to production. It can create environments on the fly. One very nice feature is to automatically create pull request environments, that would then be promoted into a production environment upon merge.

<!-- ## Infrastructure Monitoring

## Application Monitoring

## Logs Management -->

<!-- ## Encryption -->
