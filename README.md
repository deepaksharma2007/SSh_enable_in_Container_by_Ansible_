
# 🔰 Configure Webserver Inside Container By Ansible🔰

### Description 

By default docker container is isolated. So we cannot ssh the conainer. Ansible uses the ssh way to login container. So I create a docker image that has ssh enabled. So we can directly launch container and configure apache webserver within the container by Ansible Tool.

### Steps

🔹 Ansible PlayBook Configure Docker

🔹 Start and enable Docker services

🔹 Pull the docker image (deepak2007/centos_ssh) from the Docker Hub

🔹 Run the docker container and expose it to the public

🔹 Also make docker container persistent storage

🔹 Retrieve newContainer IP and update the inventory

🔹 Configure Webserver inside the docker container

#### Docker Image  :- https://hub.docker.com/r/deepak2007/centos_ssh

#### For more detail ,please visit 

