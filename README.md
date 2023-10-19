# DockerConcepts
Docker Related Concepts

## Why Docker?
Docker makes it easy to install and run software without worrying about setup or dependencies.
## What is Docker?

eccosystem of creating container
docker Images
container : instance of image

Docker Client: CLI
Docker Server: Docker Daemon -> responsible for creating images , runing containers.


Docker hub : free public repository 



- for runing dockers on machine : ```docker ps ```
- for history docker on my machine : ``` docker ps -all ```
- Docker run : ```Docker run image-name ``` docker image first find on locally if not find then fetch it from online Docker hub.
- Docker run run two commands: ```docker create imagename``` and return docker Id and then call ``` docker start id ```.
- example to play with differen images are : ```hello-word``` , ```busybox```, ```redis```

### play with redis

-   docker run redis
-   docker ps  (get containder id)
-   ```docker exec```  multi command container , Executing command in runing container
-   docker exec -it dockerId command 
-   command may be docker exec -it dockerId redis-cli
-   or open the running container shell by using ```sh```
-   docker exec -it dockerId sh  [-it = -i -t] -it get input and show to the out put
-   redis commands ```set myvalue = 5 ``` and fetch by  ```get myvalue ```
