# Docker Project

### What is Docker?
Docker is a platform that allows application to be packaged into containers

Containers are self-contained environments that include everything needed to run an application (libraries, dependencies, and configurations)
#### Advantages to using Docker:
- Portability- move applications easily between environments
- Consistency- no dependency or configuration issues
- Scalability- quickly start/stop containers
### High-level Infratsructure Design
#### Components:
- Reverse Proxy- single entry point for the application
- Load balancer- distributes traffic between two API servers
- Front-end server- serves static content to clients

#### Traffic Routing:
- Front-end- reverse proxy route requests to front-end server; client communicates only wtih reverse proxy
- API- reverse proxy routes requests to API servers using Round Robin Load Balancing

#### Round Robin Load Balancing
This distributes incoming requests evenly across multiple servers
Each server gets a turn in sequence to handle requests
Advantages are simplicity with implementation and ensures even distribution of workload among servers
May not suit all workload patterns or resource requirements, but is adequate for basic load balancing needs