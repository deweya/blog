FROM registry.redhat.io/ubi8/ubi:8.2

# Comes from an OCP secret also called ‘nexus-creds’
COPY nexus-creds nexus-creds

RUN curl -u $(cat nexus-creds/username):$(cat nexus-creds/password) -O http://example-nexusrepo-sonatype-nexus-demo.apps-crc.testing/repository/example-artifacts/jq && \
    chown :0 jq && \
    chmod 010 jq && \
    mv jq /usr/local/bin && \
    rm -rf nexus-creds