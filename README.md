# docker-cheat-sheet

## Delete all containers

```bash
  docker rm $(docker ps -a -q)
```

# Delete all images

```bash
  docker rmi $(docker images -q)
```
