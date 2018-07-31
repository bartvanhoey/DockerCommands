# Docker

## Docker Commands

| Command                                                     |               Action                                          |
|-------------------------------------------------------------|---------------------------------------------------------------|
|`docker ps`                                                  | docker running containers                                     |
|`docker ps -a`                                               | docker exited containers                                      |
|`docker run -it microsoft/windowsservercore cmd.exe`         | run windowsservercore image, run command inside container     |
|`-it`                                                        | run container in interactive mode                             |
|`-d`                                                         | run container as background process                           |

| `C:\copy con mydemofile.txt`  - `CTRL+C to exit`            | create an opens a file in command mode                        |
| `C:\type mydemofile.txt`                                    | open and read add file in command mode                        |
| `exit`                                                      | exit command prompt docker container                          |
| type `powershell` in docker container and type `get-process`| get running processes on local container                      |

If you get error message `image operating system "windows" cannot be used on this platform` you need to switch to Windows Containers on Docker -> Right Click on Docker Icon in Notification Area and choose `Switch to Windows Containers...`

| Command                                                     |               Action                                          |
|-------------------------------------------------------------|---------------------------------------------------------------|
|`docker exec <container name/container id> ipconfig`         | get the IP address of a running container                     |
|`docker ps -a`                                               | list of running containers (-a slso show exited containers)   |
|`docker images`                                              | shows the list of container images on a machine               |
|`docker network`                                             | manage networking with Docker                                 |
|`docker pull microsoft/windowsservercore`                    | pull latest windowsservercore image from Docker Hub           |

docker: Error response from daemon: failed to create endpoint xenodochial_engelbart on network nat: HNS failed with error : Unspecified error.git a