to run a interactive terminal for us container

    docker run -i $container id

To alocate a pseudo tty that is like create a temrinal

    docker run -t $containre id
    docker run -tty $container id

In combination
    
    docker run -it $container id

if we want to restart a container who need  interaction we can use

    docker start -a $container
    or 
    docker start -i $container