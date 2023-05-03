the command used on terminal has been.

docker build .

to build docker image

docker run -p 3000:3000 $docker_id

with this we run de image and asign the port 3000 (first call) to respond to port 3000 (second writed) of image the id is given after succedfully run docker build .

is the id at the end with format writing image sha256: docker_id

by default is no comutication between local machine and docker container

docker ps will list all docker container runin

docker stop $container name

will stop the running container