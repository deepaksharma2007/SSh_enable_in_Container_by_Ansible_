
# ๐ฐ Configure Webserver Inside Container By Ansible๐ฐ

### Description 

By default docker container is isolated. So we cannot ssh the conainer. Ansible uses the ssh way to login container. So I create a docker image that has ssh enabled. So we can directly launch container and configure apache webserver within the container by Ansible Tool.

### Steps

๐น Ansible PlayBook Configure Docker

๐น Start and enable Docker services

๐น Pull the docker image (deepak2007/centos_ssh) from the Docker Hub

๐น Run the docker container and expose it to the public

๐น Also make docker container persistent storage

๐น Retrieve newContainer IP and update the inventory

๐น Configure Webserver inside the docker container

#### Docker Image  :- https://hub.docker.com/r/deepak2007/centos_ssh

#### For more detail ,please visit 

