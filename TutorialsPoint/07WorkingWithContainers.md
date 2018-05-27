# Working With Containers
In this chapter, we will explore in detail what we can do with containers.

## docker top
With this command, you can see the top processes within a container.

### Syntax
```
$ docker top ContainerID
```

### Options
> - **ContainerID** - This is the Container ID for which you want to see the top processes.

### Return Value
The output will show the top-level processes within a container.

### Example
```
$ sudo docker top 9f215ed0b0d3
```

The above command will show the top-level processes within a container.

### Output
when we run the above command, it will produce the following result -

![Docker Top](/TutorialsPoint/res/img/dockek_top.jpg)

### docker stop
This command is used to stop a running container.

#### Syntax
```
$ docker stop ContainerID
```

#### Options
> - **ContainerID** - This is the Container ID which needs to be stopped.

#### Return Value
The output will give the ID of the stopped container.

#### Example
```
$ sudo docker stop 9f215ed0b0d3
```
The above command will stop the Docker container **9f215ed0b0d3**.

#### Output
When we run the above command, it will produce the following result -

![Docker Stop](/TutorialsPoint/res/img/docker_stop.jpg)

#### docker rm
This command is used to delete a container.

#### Syntax
```
$ docker rm ContainerID
```

#### Options
> - **ContainerID** - This is the Container ID which needs to be removed.

#### Return Value
The output will give the ID of the removed container.

#### Example
```
$ sudo docker rm 9f215ed0b0d3
```

The above command will remove the Docker container **9f215ed0b0d3**.

#### Output
When we run the above command, it will produce the following result -

![Docker rm](/TutorialsPoint/res/img/docker_rm.jpg)

### docker stats
This command is used to provide the statistics of a running container.

#### Syntax
```
$ docker stats ContainerID
```

#### Options
> - **ContainerID** - This is the Container ID for which the stats need to be provided.

#### Return Value
The output will show the CPU and Memory utilization of the Container.

#### Example
```
$ sudo docker stats 9f215ed0b0d3
```

The above command will provide CPU and memory utilization of the Contaer **9f215ed0b0d3**.

#### Output
When we run the above command, it will produce the following result -

![Docker stats](/TutorialsPoint/res/img/docker_stats.jpg)

### docker attach
This command is used to attach to a running container.

#### Syntax
```
$ docker attach ContainerID
```

#### Options
> - **ContainerID** - This is the Container ID to which you need to attach.

#### Return Value
None

#### Example
```
$ sudo docker attach 07b0b6f434fe
```

The above command will attach to the Docker container **07b0b6f434fe**.

#### Output
When we run the above command, it will produce the following result -

![Docker attach](/TutorialsPoint/res/img/docker_attach.jpg)

Once you have attached to the Docker container, you can run the above command to see the process utilization in that Docker container.

![Docker attach container](/TutorialsPoint/res/img/docker_attach_container.jpg)

### docker pause
This command is used to pause the processes in a running container.

#### Syntax
```
$ docker pause ContainerID
```

#### Options
> - **ContainerID** - This is the Container ID to which you need to pause the processes in the container.

#### Return Value
The ContainerID of the paused container.

#### Example
```
$ sudo docker pause 07b0b6f434fe
```

The above command will pause the processes in a running container **07b0b6f434fe**.

#### Output
When we run the above command, it will produce the following result -

![Docker pause](/TutorialsPoint/res/img/docker_pause.jpg)

### docker unpause
This command is used to **unpause** the processes in a running container.

#### Syntax
```
$ docker unpause ContainerID
```

#### Options
> - **ContainerID** - This is the Container ID to which you need to unpause the processes in the container.

#### Return Value
The ContainerID of the running container.

#### Example
```
$ sudo docker unpause 07b0b6f434fe
```

The above command will unpause the processes in a running container: 07b0b6f434fe

#### Output
When we run the above command, it will produce the following result -

![docker unpause](/TutorialsPoint/res/img/docker_unpause.jpg)


### docker kill
This command is used to kill the processes in a running container.

#### Syntax
```
$ docker kill ContainerID
```

#### Options
> - **ContainerID** - This is the container ID to which you need to kill the processes in the container.

#### Return Value
The ContainerID of the running container.

#### Example
```
$ sudo docker kill 07b0b6f434fe
```

The above command will kill the processes in the running container **07b0b6f434fe**.

#### Output
When we run the above command, it will produce the following result -

![docker kill](/TutorialsPint/res/img/docker_kill.jpg)


## Docker - Container Lifecycle
The following illustration explains the entire lifecycle of a Docker container.

![container lifecycle](/TutorialsPoint/res/img/container_lifecycle.jpg)

> - Initially, the Docker container will be in the **created** state.
> - Then the Docker container goes into the running state when the Docker **run** command is used.
> - The Docker **kill** command is used to kill an existing Docker container.
> - The Docker **pause** command is used to pause an existing Docker container.
> - The Docker **stop** command is used to pause an existing Docker container.
> - The Docker **run** command is used to put a container back from a **stopped** state to a **running** state.


