docker run -dit --name faleconosco --hostname faleconosco -v $(pwd):/usr/src -w /usr/src node:18

docker exec -it faleconosco /bin/bash