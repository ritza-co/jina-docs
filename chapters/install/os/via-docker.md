# Install Jina via Docker Container

The simplest way to use Jina is via Docker. We provide a universal container image as small as 100MB that can be run on multiple architectures without worrying about package dependencies. Of course, you need to have [Docker installed](https://docs.docker.com/install/) first.

## Running Jina image

```bash
docker run jinaai/jina:latest
```

This command downloads the latest Jina image from [Docker Hub](https://hub.docker.com/r/jinaai/jina/tags) based on your local architecture and then runs it in a container. When the container runs, it prints a help message and exits.

### Supported architectures

This Docker image is based on `python:3.7.6-slim` and can be run on the following CPU architectures:

- amd64
- arm64
- ppc64le
- 386
- arm/v7
- arm/v6

No extra steps are required to run on the above architectures, simply run `docker run jinaai/jina`

## Running Jina development or pre-release

The following command will run the latest version of Jina from the GitHub master branch. Be aware this version may be unstable and should only be used to test new features.

```bash
docker run jinaai/jina:master
```
