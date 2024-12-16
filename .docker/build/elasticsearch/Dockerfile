# syntax = docker/dockerfile:1.0-experimental
# production stage
ARG ELASTIC_PORT

FROM olelarsen/elastic-setup:latest

RUN sysctl -w vm.max_map_count=280530

CMD ["elasticsearch"]

EXPOSE $ELASTIC_PORT