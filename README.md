# docker-cheat-sheet

## Delete all containers

```bash
  docker rm $(docker ps -a -q)
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

## Dump logs of docker compose env  

```bash
docker-compose logs --no-color >& logs.log
```
## Login into container

```bash
docker exec -i -t {{containerID}} /bin/bash
```

## List all images

```bash
docker images --all
```

## Delete all images

```bash
  docker rmi $(docker images --quiet --all)
```

## Remove all exited containers

###  list:

```bash
  docker ps -a -f status=exited
```

### Remove:
```bash
  docker rm $(docker ps -a -f status=exited -q)
```
