# Containers
Containers are instances of Docker images that can be run using the Docker run command. The basic purpose of Docker is to run containers. Let's discuss how to work with containers.

## Running a Container
Running of containers is managedwith the Docker **run** command. To run a container in an interactive mode, first launch the Docker container.

```
$ sudo docker run -it centos /bin/bash
```

Then hit Ctrl+p and you will return to your OS shell

![Containers](/TutorialsPoint/res/img/containers.jpg)

You will then be running in the instance of the CentOS system on the Ubuntu server.

## Listing of Containers
One can list all of the containers on the machine via the **docker ps** command. This command is used to return the currently running containers.

```
$ docker ps
```

### Syntax
```
$ docker ps
```

### Options
None

### Return Value
The output will show the currently running containers.

### Example
```
$ sudo docker ps
```

### Output
When we run the above command, it will produce the following result -

![Listing of Containers](/TutorialsPoint/res/img/listing_of_containers.jpg)

Let's see some more variations of the **docker ps** command.

## docker ps -a
This command is used to list all of the containers on the system

### Syntax
```
$ docker ps -a
```

### Options
> - **-a** - It tells the **docker ps** command to list all of the containers on the system.

### Return Value
The output will show all containers.

### Example
```
$ sudo docker ps -a
```

### Output
when we run the above command, it will produce the following result -

![Docker ps -a](/TutorialsPoint/res/img/docker_ps_a.jpg)

## docker history
With this command, you can see all the commands that were run with an image via a container.

### Syntax
```
$ docker history ImageID
```

### Options
> - **ImageID** - This is the Image ID for which you want to see all the commands that were run against it.

### Return Value
The output will show all the commands run against that image.

### Example
```
$ sudo docker history centos
```

The above command will show all the commands that were run against the **centos** image.

### Output
When we run the above command, it will produce the following result -

![Docker History](/TutorialsPoint/res/img/docker_history.jpg)

