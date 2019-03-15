# Docker

## Docker Commands

| Command                                                     |               Action                                          |
|-------------------------------------------------------------|---------------------------------------------------------------|
|`docker ps`                                                  | docker running containers                                     |
|`docker ps -a`                                               | docker exited containers                                      |
|`docker run -it microsoft/windowsservercore cmd.exe          | run windowsservercore image, run command inside container     |

If you get error message `image operating system "windows" cannot be used on this platform` you need to switch to
Windows Containers on Docker -> Right Click on Docker Icon in Notification Area and choose `Switch to Windows Containers...`

| Command                                                     |               Action                                          |
|-------------------------------------------------------------|---------------------------------------------------------------|
|`docker exec <container name> ipconfig`                      | get the IP address of a running container                     |
|`docker ps -a`                                               | list of running containers (-a slso show exited containers)   |
|`docker images`                                              | shows the list of container images on a machine               |
|`docker network`                                             | manage networking with Docker                                 |
|`docker pull microsoft/windowsservercore`                    | pull latest windowsservercore image from Docker Hub           |
|`docker rm <CONTAINER ID>`                                   | remove a specific container                                   |
|`docker rm -f <CONTAINER ID>`                                | remove a specific running container                           |
|`docker system prune`                                        | clean up any resources — images, containers, volumes and      |
|                                                             | network sthat are dangling (not associated with a container)  |
|`docker system prune -a`                                     | to additionally remove any stopped containers and all unused  |
|                                                             | images (not just dangling images)                             |
|`docker rmi <IMAGE ID>`                                      | remove image                                                  |

 ATTENTION: You may get error like: Error response from daemon: conflict: unable to remove repository reference IMAGE NAME
 (must force) - container 302e8bd is using its referenced image 3334b287844 -> a stopped container isn't actually removed.

## Docker Parameters

| Parameter                                                   |               Description                                     |
|-------------------------------------------------------------|---------------------------------------------------------------|
|`-d`                                                         | detached, when you need to run a background service.          |
|`-p` 8080:80                                                 | expose inside container port 80 to port 8080 on your machine  |
|`--rm`                                                       | removes the container from list after container has stopped   |
