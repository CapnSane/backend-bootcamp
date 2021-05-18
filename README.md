# Backend Bootcamp
</br>
## About it

This repository is part of a Backend Learning Project offered b [Ingate Educa](https://ingate.com.br/) and signed to me by [Yoyo Sensei](https://github.com/yoannes) from Japan.

The main goal is creating a the backend environment for implementing the card game marketplace developed using the Vue.js framework as the final project of the last Vue Ingate class.

### What will be seen in this course?

#### 1. Docker
- Images
- Containers
- Container-Orchestration (docker-compose)
</br>

#### 2. Database (mySQL)
- ERD - entity relationship diagram
- Database management ([TablePlus](https://tableplus.com/))
</br>

#### 3. REST API (node.js)
- [Express.js](https://expressjs.com/) (web framework)
- [Objection.js](https://vincit.github.io/objection.js/) (ORM)
- API Documentation ([Stoplight](https://stoplight.io/))
- API creation
    - Test creation ([Mocha](https://mochajs.org/))
    - Route creation
    - Models creation

## 1. Docker
### What is Docker?
Docker is a set of platform as a service (PaaS) products that use OS-level virtualization to deliver software in packages called containers.

### What are Containers?
Containers are isolated from one another and bundle their own software, libraries and configuration files; they can communicate with each other through well-defined channels.

### What is Docker image?
A Docker image is a read-only template used to build containers. Images are used to store and ship applications.

### What is the main advantage of using Docker?
Because all of the containers share the services of a single operating system kernel, they use fewer resources than virtual machines.

### What else?
When virtual machines are used, they spend lots of gigabytes in operational systems, which are fully installed. Another thing is that virtual machines still take too much time in their provisioning and have a limited portability. Working with Docker it is possible to isolate a single application and its dependencies, besides enabling more efficient use of system resources.

### What is container-orchestration?

The container-orchestration aims to provide a "platform for automating deployment, scaling, and operations of application containers across clusters of hosts".

We will work with Docker Compose, that is a tool for defining and running multi-container Docker applications. With Compose, you use a YAML file to configure your application’s services. Then, with a single command, you create and start all the services from your configuration. 

Basically, the container-orchestration provides:
  - Provisioning and deployment
  - Configuration and scheduling 
  - Resource allocation
  - Container availability
  - Scaling or removing containers based on workloads
  - Traffic routing 
  - Monitoring
  - Applications configuration
  - Containers security