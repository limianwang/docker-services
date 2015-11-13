# docker-services
Generic Dockerfile for services I use.

# Pushing to private docker registry

```
docker tag -f {NAME}:{TAG} {REPOSITORY}/{NAME}
docker push {REPOSITORY}/{NAME}:{TAG}
```
