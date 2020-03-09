FROM debian:buster-slim
ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update
RUN apt-get install -y \
    apt-utils \
    curl \
    git \
    tree \
    tmux

WORKDIR /app

RUN groupadd -g 1000 appuser && \
    useradd -r -u 1000 -g appuser appuser
RUN chown appuser.appuser /app

# USER appuser

# COPY executable_name .
# ENTRYPOINT ["/app/executable_name"]
