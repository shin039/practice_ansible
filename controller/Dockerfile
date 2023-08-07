ARG CENTOS_VER
ARG APP_PATH

FROM centos:${CENTOS_VER}

WORKDIR ${APP_PATH}

RUN yum install -y epel-release \
    && yum install -y ansible openssh sshpass openssh-clients

CMD ["/sbin/init"]
