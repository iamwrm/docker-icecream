FROM ubuntu:20.04

RUN apt-get update && apt-get install -y \
    icecc

# Run icecc daemon in very verbose mode with default name `docker-compiler`
ENTRYPOINT ["iceccd","-vv","-N","docker-compiler"]

# Expose required TCP/UDP ports
EXPOSE 10245 8765/TCP 8765/UDP 8766