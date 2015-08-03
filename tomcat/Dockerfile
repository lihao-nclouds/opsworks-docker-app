From centos:6
ENV HOME="/root"
RUN yum clean all && \
    yum -y install epel-release && \
    yum -y install openssh-server git sudo 
RUN service sshd start
EXPOSE 22
CMD ["/usr/sbin/sshd", "-D"]
