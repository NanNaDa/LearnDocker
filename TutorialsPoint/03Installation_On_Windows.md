Let's go through the installation of each product.

# Docker for Windows
Once the installer has been downloaded, double-click it to start the installer and then follow the steps given below.
> ### Step 1 
> Click on the Agreement terms and then the Install button to proceed ahead with the installation.
>
> ![docker setup](/TutorialsPoint/res/img/docker_setup.jpg)
>
> ### Step 2
> Once complete, click the Finish button to complete the installation.
> 
> ![docker finish](/TutorialsPoint/res/img/finish.jpg)

## Docker ToolBox
Once the installer has been downloaded, double-click it to start the installer and then follow the steps given below.
>
> ### Step 1
> Click the Next button on the start screen.
>
> ![Docker Toolbox Next](/TutorialsPoint/res/img/docker_toolbox_next.jpg)
> 
> ### Step 2
> Keep the default location on the next screen and click the Next button.
> 
> ![Destination Location](/TutorialsPoint/res/img/destination_location.jpg)
>
> ##### Step 3
> Keep the default components and click the Next button to proceed.
> 
> ![Select Components](/TutorialsPoint/res/img/select_components.jpg)
>
> ### Step 4
> Keep the Additional Tasks as they are and then click the Next button.
> 
> ![Additional Tasks](/TutorialsPoint/res/img/additional_tasks.jpg)
>
> ### Step 5
> On the final screen, click the Install button.
> 
> ![Install](/TutorialsPoint/res/img/install.jpg)
>

## Working with Docker Toolbox
Let's now look at how Docker Toolbox can be used to work with Docker containers on Windows. The first step is to launch the Docker Toolbox application for which the shortcut is created on the desktop when the installation of Docker toolbox is carried out.

![Quick Start Terminal](/TutorialsPoint/res/img/quickstart_terminal.jpg)

Next, you will see the configuration being carried out when Docker toolbox is launched.

![Docker Toolbox Launched](/TutorialsPoint/res/img/docker_toolbox_launched.jpg)

Once done, you will see Docker configured and launched. You will get an interactive shell for Docker.

![Interactive Shell](/TutorialsPoint/res/img/interactive_shell.jpg)

To test that Docker runs properly, we can use the Docker **run command** to download and run a simple **HelloWorld Docker container**.

The working of the Docker **run command** is given below -

```
$ docker run
```

This command is used to run a command in a Docker container.

### Syntax
```
$ docker run image
```

### Options
- **Image** - This is the name of the image which is used to run the container.

### Return Value
The output will run the command in the desired container.

### Example
```
$ sudo docker run hello-world
```

This command will download the **hello-world** image, if it is not already present, and run the **hello-world** as a container.

### Output
When we run the above command, we will get the following result -

![Docker Container](/TutorialsPoint/res/img/docker_container.jpg)

If you want to run the Ubuntu OS on Windows, you can download the Ubuntu Image using the following command -
```
$ Docker run -it Ubuntu bash
```

Here you are telling Docker to run the command in the interactive mode via the **-it** option.

![Ubuntu Image](/TutorialsPoint/res/img/ubuntu_image.jpg)

In the output you can see that the Ubuntu image is downloaded and run and then you will be logged in as a root user in the Ubuntu container.


