# syntax = docker/dockerfile:1.0-experimental
## production stage
ARG STACK_VERSION
ARG KIBANA_PORT
FROM docker.elastic.co/kibana/kibana:$STACK_VERSION
EXPOSE $KIBANA_PORT

ENTRYPOINT ["/bin/tini", "--"]


CMD ["/usr/local/bin/kibana-docker"]


USER kibana