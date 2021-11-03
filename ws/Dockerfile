FROM centos:latest

RUN yum install net-tools openssh-server -y

RUN ssh-keygen  -A

RUN yum install passwd -y

RUN echo redhat | passwd root --stdin

EXPOSE 80

ENTRYPOINT ["/usr/sbin/sshd"]

CMD ["-D"]
