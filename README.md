# Docker comannds:
// list running continer 
docker ps
// list all continers
docker ps-a
docker run <contianer name>
docker stop <contianer name>
docker rename <old> <new>
// -d to run in background 
// nginx 
// -it intaractive tty 
docker run --name=web -d nginx 
// excute ls /var command in nginx contianer
docker exec nginx ls /var
// 
ip a 
// to read log of contianer
docker logs nginx
// keep logs running
docker logs -f nginx
// search
docker logs -f nginx | grep favicon.ico
//
docker logs --tail -f nginx | grep favicon.ico
//copy file from diffrent directory
docker cp nginx:/etc/nginx/nginx.conf .

// hub.docker.com to show list of images

// docker pull php to install image for php contianer
docker pull php
// login to private 
docker login <private registrary>
// 
docker commit <contianer_name> <image_name>

docker rm debian

docker rmi <contiane_image> <tag> 

// redis : nonsql object to save in 










