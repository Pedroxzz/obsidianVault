
docker run -dit --name residencial --hostname residencial -v $(pwd):/usr/src -w /usr/src node:18

docker exec -it residencial bash
