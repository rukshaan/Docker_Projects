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
    docker exec -it <container name> node
windows-cmd  same as container access-bash
    docker exec -it gifted_burnell bin/bash

root@5af759efd934:/# ls
bin  boot  dev  etc  home  lib  lib64  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
root@5af759efd934:/# cd usr/local/bin
root@5af759efd934:/usr/local/bin# ls
corepack  docker-entrypoint.sh  node  nodejs  npm  npx  yarn  yarnpkg

C:\Users\gebruiker FOM011\Desktop\rukshan\Docker_Projects\docker_startup>docker run --name node_image node

C:\Users\gebruiker FOM011\Desktop\rukshan\Docker_Projects\docker_startup>docker rename  node_image my_node_images

running container only save others delete
    docker container prune 

copy file to container
 . 


C:\Users\gebruiker FOM011\Desktop\rukshan\Docker_Projects>dir
 Volume in drive C has no label.
 Volume Serial Number is 1296-D793

 Directory of C:\Users\gebruiker FOM011\Desktop\rukshan\Docker_Projects

04/26/2025  12:41 PM    <DIR>          .
04/25/2025  05:59 PM    <DIR>          ..
04/25/2025  06:28 PM    <DIR>          docker_startup
04/26/2025  12:41 PM                 0 example1.txt.txt
               1 File(s)              0 bytes
               3 Dir(s)  127,381,725,184 bytes free


C:\Users\gebruiker FOM011\Desktop\rukshan\Docker_Projects>docker cp .\example1.txt.txt my_alpine_container:/Example.txt
Successfully copied 1.54kB to my_alpine_container:/Example.txt

C:\Users\gebruiker FOM011\Desktop\rukshan\Docker_Projects\docker_startup>docker cp my_alpine_container:/Example.txt ./example_copy.txt
Successfully copied 1.54kB to C:\Users\gebruiker FOM011\Desktop\rukshan\Docker_Projects\docker_startup\example_copy.txt












