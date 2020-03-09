FROM debian:buster-slim
ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update
RUN apt-get install -y \
    apt-utils \
    curl \
    git \
    tree \
    tmux

RUN apt-get install -y \
    python3-dev python3-pip

RUN pip3 install --upgrade pip

RUN cd /usr/local/bin && \
    ln -s /usr/bin/python3 python

WORKDIR /app

RUN groupadd -g 1000 appuser && \
    useradd -r -u 1000 -g appuser appuser
RUN chown appuser.appuser /app

# USER appuser

# COPY executable_name .
# ENTRYPOINT ["/app/executable_name"]
