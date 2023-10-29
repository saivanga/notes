### Docker

#### Manage Containers

1. Start a new container
   ```
   sudo docker container run -it --name <container_name> <image_name> <shell>
   ```
   Example:
   - To start a new interactive container with ubuntu operating system with the name ubuntu and bash as shell
     ```
     sudo docker container run -it --name ubuntu ubuntu bash
     ```

```
List currently running containers
* sudo docker container ls
List all containers including stopped
* sudo docker container ls -a
Remove any existing stopped container
* sudo docker container rm <container_id_or_container_name>

Questions
* What happens if you try to use the above command on a container that is currently running?
* Is there a purge command in docker? What does it do? When can we use that?
* How can I run an nginx server from docker?
* How can I force remove a container that is already running?
* Create a new linux.md file.
* List useful linux commands
   * find command
   * grep command
   * how do I know what OS, version and it's architecture of the currently logged in container?
   * how do I list all the currently running services/processes
```

```
Managing Images
*
```
