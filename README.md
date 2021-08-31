// remove all container
docker rm -f $(docker ps -a -q)

//remove all images
docker rmi -f $(docker images -a -q)

//remove all volumes
docker volume rm $(docker volume ls -q)