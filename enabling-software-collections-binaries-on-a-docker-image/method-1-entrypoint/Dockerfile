FROM docker.io/centos:7

# Install SCL release package and python SCL
RUN yum -y install centos-release-scl && \
    yum -y install --setopt=tsflags=nodocs rh-python35

# Enable rh-python scl binary
COPY entrypoint.sh /usr/bin/entrypoint.sh
RUN chmod +x /usr/bin/entrypoint.sh
ENTRYPOINT [ "/usr/bin/entrypoint.sh" ]