# Docker Erlang
## https://github.com/dylanngo95/docker-erlang


## What is Erlang?
Erlang is a programming language used to build massively scalable soft real-time systems with requirements on high availability. Some of its uses are in telecoms, banking, e-commerce, computer telephony and instant messaging. Erlang's runtime system has built-in support for concurrency, distribution and fault tolerance.

## TL;DR

```console
docker run -it --name erlang -v /path/to/app:/home/erlang/app dylanops/erlang
```

## Supported tags and respective Dockerfile links

Learn more about the DylanOps tagging policy and the difference between rolling tags and immutable tags [in our documentation page](https://jundat95.com/).

* [`22.3.4.21-slim`, `22.3.4.21-rebar3` (22/slim/Dockerfile)](https://github.com/dylanngo95/docker-erlang/22/slim/Dockerfile)


# Get this image

The recommended way to get the DylanOps Erlang Docker Image is to pull the prebuilt image from the [Docker Hub Registry](https://hub.docker.com/r/dylanops/erlang).

```console
$ docker pull dylanops/erlang:latest
```

To use a specific version, you can pull a versioned tag. You can view the [list of available versions](https://hub.docker.com/r/dylanops/erlang/tags/) in the Docker Hub Registry.

```console
$ docker pull dylanops/erlang:[TAG]
```

Using Docker Compose:

```yaml
version: '2'
services:
  erlang:
    image: 'dylanops/erlang:latest'
    networks:
      - app-tier
    volumes:
      - /path/to/app:/home/erlang/app
networks:
  app-tier:
    driver: bridge
```