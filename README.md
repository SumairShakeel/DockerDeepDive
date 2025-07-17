### DockerDeepDive Learning Modules:
**🔸 Installation and Configuration:**    
 Sizing Requirements
 • Docker Engine Installation
 • Swarm Installation
 • Docker Enterprise – UCP, DTR
 • Manage Users & Teams
 • Daemon Configuration
 • Certificate based auth
 • Namespaces & Cgroups
 • Troubleshoot issues
 • Configure Backups

**🔸 Image Management:**

Dockerfile
• Dockerfile Instructions
• Create efficient image
• Docker Image CLI
• Push,Pull,Delete images
• Inspect Images
• Tag Images
• Display Layers
• Registry Functions
• Deploy & Search in Registry

**🔸 Storage and Volumes:**

Drivers for various OS
• Compare Objects vs Block
• Image layers and filesystem
• Volumes
• Cleanup unused images
• PV, PVCs on Kubernetes
• Storage Classes

**🔸Networking:**

Container Network Model
• Built-in Network Drivers
• Traffic flow between Docker Engine, Registry & UCP
• Docker Bridge Network
• Publish Ports
• External DNS
• Deploy a service on a docker overlay network
• Troubleshoot container and engine logs
• Kubernetes traffic using Cluster IP and NodePort Services
• Kubernetes Network Policies

**🔸Security:**

Image signing
• Docker Engine Security
• Docker Swarm Security
• Identity Roles
• UCP Workers vs Managers
• Security scan in images
• Docker Content Trust
• RBAC with UCP
• UCP with LDAP/AD
• UCP Client Bundles

**🔸Orchestration:**

Docker Swarm:
• Setup Swarm Cluster
• Quorum in a Swarm Cluster
• Stack in swarm
• Scale up and down replicas
• Networks, Publish Ports
• Replicated vs Global Services
• Placements
• Healthchecks
• Kubernetes
• PODS, Deployments
• Services
• ConfigMaps, Secrets
• Liveness and Readiness Probes

 **Pull image from Docker Registry:**
 
 $ docker image pull alpine

Alpine image is a lightweight image that can be used as a base image.

**List the images:**

$ docker image ls

REPOSITORY                 TAG       IMAGE ID       CREATED         SIZE

sumairshakeel/myhubimage   v2        22f4e4d8dc23   4 weeks ago     7.79MB

sumairshakeel/myhubimage   v3        22f4e4d8dc23   4 weeks ago     7.79MB

fisrtimage                 latest    22f4e4d8dc23   4 weeks ago     7.79MB

mysecondimage              v1        22f4e4d8dc23   4 weeks ago     7.79MB

alpine                     latest    1d34ffeaf190   7 weeks ago     7.79MB

busybox                    latest    65ad0d468eb1   13 months ago   4.26MB

hello-world                latest    d2c94e258dcb   14 months ago   13.3kB


**Delete Images:**
$ sudo docker rmi 22f4e4d8dc23 

The above command end shows the image id, to delete the image with its id.

**Forcefully Delete Images:**

sudo docker rmi -f   d2c94e258dcb 

The image can be used as a base image to create any container, but we can delete it. 

**Port Mapping in Docker:**

There are many reasons we do port mapping, for example accessing running services inside the container with port number and IP address from the local host server to the docker container, security is also important.



