ARG CENTOS_VER
ARG APP_PATH

FROM centos:${CENTOS_VER}

WORKDIR ${APP_PATH}

# パッケージのインストール
RUN yum install -y sudo \
    && yum install -y epel-release \
    && yum install -y openssh-server

# 作業ユーザ追加
RUN useradd -G wheel -m ansible -s /bin/bash \
    && echo "ansible:ansible" | chpasswd

CMD ["/sbin/init"]
