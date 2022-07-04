# CNC - Yousaf - 2022/06/26

## CLOUD NATIVE COMPUTING

### CONTAINERS

- A Container is a runtime instance of an image
- An Image is an executable package that includes everything needed to run an application
  - the code,
  - a runtime,
  - Libraries,
  - environment variables,
  - and configuration files
- Making a container using image for any application is called Containerization
- Docker is widely use to containerize your application

### CONTAINERIZATION

- Containerization is increasingly popular because containers are:
  - Flexible: Even the most complex applications can be containerized.
  - Lightweight: Containers leverage and share the host kernel.
  - Interchangeable: You can deploy updates and upgrades on-the-fly.
  - Portable: You can build locally, deploy to the cloud, and run anywhere.
  - Scalable: You can increase and automatically distribute container replicas.
  - Stackable: You can stack services vertically and on-the-fly

### ORCHESTRATION

- Deploying your application with all dependencies into a container is just the first step
- Every ease comes with it’s own challenges, making app containerized solves the deployment problems you had previously, but new challenges includes
- Scaling app based on the current load of your system isn’t that easy. You need to
  - monitor your system,
  - trigger the startup or shutdown of a container,
  - make sure that all required configuration parameters are in place,
  - balance the load between the active application instances
  - share authentication secrets between your containers
- Doing all of that manually requires a lot of effort and is too slow to react to unexpected changes in system load
- You need to have the right tools in place that automatically do all of this
- This is what the different orchestration solutions are built for
- One of the most popular one is Kubernetes

### CONTINUOUS INTEGRATION / CONTINUOUS DELIVERY - DEPLOYENT

- CI/CD is a method to frequently deliver apps to customers by introducing automation into the stages of app development
- The main concepts attributed to CI/CD are
  - CI is Continuous Integration,
  - The “CD” refers to continuous delivery and/or continuous deployment
- CI/CD is a solution to the problems integrating new code can cause for development and operations teams
- Specifically, CI/CD introduces ongoing automation and continuous monitoring throughout the lifecycle of apps, from integration and testing phases to delivery and deployment
- Taken together, these connected practices are often referred to as a “CI/CD pipeline”
- Jenkins is most popular tool used for CI/CD

| Continuous Integration | Continuous Delivery   | Continuous Deployment |
| ---------------------- | --------------------- | --------------------- |
| build                  | Release to repository | deploy to production  |
| test                   |                       |                       |
| merge                  |                       |                       |

- Continuous Integration (CI)
  - is an automation process for developers. Successful CI means new code changes to an app are regularly built, tested, and merged to a shared repository
- Continuous Delivery
  - usually means a developer’s changes to an application are automatically bug tested and uploaded to a repository (like GitHub or a container registry), where they can then be deployed to a live production environment
- Continuous Deployment (the other possible “CD”)
  - can refer to automatically releasing a developer’s changes from the repository to production, where it is usable by customers
