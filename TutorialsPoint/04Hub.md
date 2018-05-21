# Docker - Hub
Docker Hub is a registry service on the cloud that allows you to download Docker images that are built by other communities. You can also upload your own Docker built images to Docker hub. In this chapter, we will see how to download and the use the Jenkins Docker image from Docker hub.

The official site for Docker hub is - https://www.docker.com/community-edition#add_ons

> ### Step 1
> First you need t do a simple sign-up on Docker hub.
> 
> ![Docker Hub Signup](/TutorialsPoint/res/img/docker_hub_signup.jpg)
>
> ### Step 2
> Once you have signed up, you will be logged into Docker Hub.
> 
> ![Logged Into Docker Hub](/TutorialsPoint/res/img/logged_into_docker_hub.jpg)
>
> ### Step 3
> Next, let's browse and find the Jenkins image.
> 
> ![Jenkins Image](/TutorialsPoint/res/img/jenkins_image.jpg)
>
> ### Step 4
> If you scroll down on the same page, you can see the Docker **pull** command. This will be used to download the Jenkins image onto the local Ubuntu server.
>
> ![Pull Command](/TutorialsPoint/res/img/pull_command.jpg)
> 
> ### Step 5
> Now, go to the Ubuntu server and run the following command -
> 
> ```
> $ sudo docker pull jenkins
> ```
> 
> ![Ubuntu Server](/TutorialsPoint/res/img/ubuntu_server.jpg)
>
> To run Jenkins, you need to run the following command -
>
> ```
> $ sudo docker run -p 8080:8080 -p 50000:50000 jenkins
> ```
>
> Note the following points about the above **sudo** command -
> - We are using the **sudo** command to ensure it runs with root access.
> - Here, **jenkins** is the name of the image we want to download from Docker hub and install on our Ubuntu machine.
> - **-p** is used to map the port number of the internal Docker image to our main Ubuntu server so that we can access the container accordingly.
>
> ![Sudo Command](/TutorialsPoint/res/img/sudo_command.jpg)
>
> You will then have Jenkins successfully running as a container on the Ubuntu machine.
