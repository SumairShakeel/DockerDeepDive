### DockerDeepDive Learning Modules:

**Installation and Configuration**
 - Sizing Requirements
 - Docker Engine Installation
 - Swarm Installation
 - Docker Enterprise – UCP, DTR
 - Manage Users & Teams
 - Daemon Configuration
 - Certificate-based auth
 - Namespaces & Cgroups
 - Troubleshoot issues
 - Configure Backups

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



