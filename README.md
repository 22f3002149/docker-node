# Playing around with Docker

This repo is me learning docker and testing it out.
The test docker image is hosted on
[docker](https://hub.docker.com/repository/docker/sayang2001/docker-node/general).

Things I learnt during this exercise:

- What is Docker
- How it works
- What are containers
- What are images
- How to pull images
- How to build custom images using `Dockerfile`
- What is docker-compose
- How to orchestrate multiple container dependencies using `docker compose up`
- What are volumes
- How docker networking works
  - Bridge network
  - Host network
  - Custom networks
  - Pinging containers with name or IP
- Mounting volumes for non-volatile storage and sharing of data
- Port mappings (not required for host network)
- Docker Desktop
- Dockerhub
- How to push images to dockerhub
- Layering of dockerfile
- Caching of layers
- Optimizing layers for caching
- Multi-stage builds
  - Splitting image into multiple stages
  - Build stage and runner stage
  - COPY --from=build
  - WORKDIR
- Buildx from BuildKit
  - correct dependency resolution of multi-stage

---

## Run it

Run it using two steps

```bash
docker pull sayang2001/docker-node:latest
docker run -it -p 8000:8000 sayang2001/docker-node:latest
```
