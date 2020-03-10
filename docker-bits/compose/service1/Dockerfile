FROM debian:buster-slim
ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update
RUN apt-get install -y mini-httpd

WORKDIR /app
RUN touch service1.txt

RUN groupadd -g 1000 appuser && \
    useradd -r -u 1000 -g appuser appuser
RUN chown appuser.appuser /app

USER appuser
