# docker

we can restart a stopped container with 
    docker ps -a
    docker start $container id or name
this will start the container in background(detach mode)
by dafult the process with docker run are in foreground (attached mode)
if we want to launch a caontainer with in detached mnode we must add -d
docker run -p 8000:80 -d $image id

to attach terminal to certain container running we use docker container attach $container_name or id

we can also use 
    docker log $contianer nname
this will give us all the log of the ocntainer, also if we add -f it will attach
    docker log -f $container name 

    docker start -a $container name
will restart de contaider in attach mode

with 
    docker rm $container name
we can remove unused containers

to list iamges
    docker images

to delete images
    docker rmi $image id

to remove al unused iamges
    docker image prune

if we use
    docker run --rm $image id
one tme the container stops will be removed

with 
    docker image inspect $image id
we will see all information about image 

to copy files from and into de container 
    docker cp $path_in_local $container_name:$container path
or
    docker cp $container_name:$container path $path_in_local 

we can give a name to containers if we ad the option --name $disired_name to the docker run command

in docker images we can define names and tags
the name help ups to create a general group
and with the tag we can be more especific 

To created a named image
    docker build -t $image_name:$image_tag . 

To removed al imaged included de tagged ones 
    docker image prune -a

