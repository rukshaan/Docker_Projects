# Docker_Projects


check =>   docker --version
details => docker info
pull image => docker pull hello-world
show images => docker images
run container => docker run hello-world
display container => docker ps -a
display running container => docker ps 

//create an image
create file Dockerfile
    #use abase image
    FROM alpine:latest

    # run a command to update the package list and install the required packages
    CMD ["echo", "Hello, Docker!"]

build a file
    docker build -t my-simple_image.


run a file
    docker run my-simple_image.


//pull a docker image 
docker pull node

check =>   docker images
run=> docker start  <container name>

    docker run -it run
        i-interactive
        t-terminal

stop container
    docker stop <id name>

use existing container
    docker start <container name>

running commands in containers
