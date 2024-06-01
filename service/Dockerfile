FROM mitmproxy/mitmproxy

ARG MITM_ID
ARG MITM_PASS

# system
RUN apt update -y -q && DEBIAN_FRONTEND=noninteractive apt install -y -q --no-install-recommends \
    apache2-utils vim \
    && rm -rf /var/lib/apt/lists/*

#RUN htpasswd
WORKDIR /etc/mitmproxy/
RUN htpasswd -bcB mitm.htpasswd ${MITM_ID} ${MITM_PASS}
WORKDIR /home/mitmproxy/

# shell
CMD ["/bin/bash"]
