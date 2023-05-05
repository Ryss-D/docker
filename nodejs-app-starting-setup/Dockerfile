#the from command allow us to create a image from a preexisting one
FROM node:14

## by default they will be running in the root 
## but with workdir we can change it
WORKDIR /app

#here we tells docker what files from project comes to image, first local machine and then the image
COPY . /app

##we will run command from "image terminal"
RUN npm install

##with expose we can expose a certain port from container to local system
EXPOSE 80
##it do not expose by selft
## we have to run the container with
## docker run -p $localport:$containerport $iuamge id
##-p means publish ig 3000:80

## the differences between run and cmd is that
##cmd will just run when a container is created from image
CMD ["node", "server.js"]
