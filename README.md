# docker-cheat-sheet

## Delete all containers

```bash
  docker rm $(docker ps -a -q)
```

## Delete all images

```bash
  docker rmi $(docker images -q)
```

## Stop all containers:

```bash
docker kill $(docker ps -q)
```

## Show logs of container 

```bash
docker logs {containerID}
```

## Show stats of container 

```bash
docker stats {containerID}
```
