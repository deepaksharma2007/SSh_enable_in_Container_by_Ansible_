
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

If we are facing issue while creating docker image due to "Error: Failed to download metadata for repo 'appstream': Cannot prepare internal mirrorlist: No URLs in mirrorlist" ,then we need to add below commands in our Docker file 


###### sed -i 's/mirrorlist/#mirrorlist/g' /etc/yum.repos.d/CentOS-*
###### sed -i 's|#baseurl=http://mirror.centos.org|baseurl=http://vault.centos.org|g' /etc/yum.repos.d/CentOS-*
###### dnf distro-sync
