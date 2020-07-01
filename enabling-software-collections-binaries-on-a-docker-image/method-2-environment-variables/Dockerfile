FROM docker.io/centos:7
 
# Install SCL release package and python SCL
RUN yum -y install centos-release-scl && \
    yum -y install --setopt=tsflags=nodocs rh-python35
 
# Enable rh-python scl binary
COPY scl_enable /usr/bin/scl_enable
ENV BASH_ENV="/usr/bin/scl_enable" \
    ENV="/usr/bin/scl_enable" \
    PROMPT_COMMAND=". /usr/bin/scl_enable"