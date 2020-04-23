from ubuntu:bionic

VOLUME /root/.swiftcash

RUN apt update -y && \
    apt install -y software-properties-common && \
    apt clean -qy

RUN add-apt-repository -y ppa:swiftcash/ppa && \
    add-apt-repository -y ppa:bitcoin/bitcoin && \
    apt install -y swiftcashd && \
    apt clean -qy

WORKDIR /root/.swiftcash

CMD [ "swiftcashd" ]
