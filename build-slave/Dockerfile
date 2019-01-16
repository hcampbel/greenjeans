FROM centos:7.6.1810

USER root


RUN yum makecache && \
    yum upgrade -y --nogpgcheck && \
    yum group install "Development Tools" -y --nogpgcheck && \
    yum install curl wget java-1.8.0-openjdk valgrind -y  --nogpgcheck && \
    yum clean all


CMD ["sh"]