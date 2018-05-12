# Installing Docker on Linux
To start the installation of Docker, we are going to use an Ubuntu instance. You can use Oracle Virtual Box to setup a virtual Linux instance, in case you don't have it already.

The following screenshot shows a simple Ubuntu server which has been installed on Oracle Virtual Box. There is an OS user named <b>demo</b> which has been defined on the system having entire root access to the server.

![a picture of demo example](/TutorialsPoint/res/img/demo_button.jpg)

To install Docker, we need to follow the steps given below.

> ## Step 1.
> Before installing Docker, you first have to ensure that you have the right Linux kernel version running. Docker is only designed to run on Linux kernel version 3.8 and higher. We can do this by running the following command.
>> ### uname
>> This method returns the system informtion about the linux system.
>>
>> ### Syntax
>> ```
>> uname -a
>> ```
>> ### Options
>> <b>a</b> - This is used to ensure that the system information is returned.
>> ### Return Value
>>This method returns the following information on the Linux system
>> - kernel name
>> - node name
>> - kernel release
>> - machine
>> - processor
>> - hardware platform
>> - operating system
>>
>> ### Example
>> ```
>> uname -a
>> ```
>> ### Output
>> When we run above command, we will get the following result
>> ![result of command](/TutorialsPoint/res/img/output.jpg)
>>
>> From the output, we can see that the Linux kernel version is 4.2.0-27 which is higher than version 3.8, so we are good to go.
>
> ## Step 2.
> You need to update the OS with the latest packages, which can be done via the following command
>> ```
>> apt-get
>> ```
>> This method installs packages from the Internet on to the Linux system.
>> ### Systax
>> sudo apt-get update
>> ### Options
>>> - <b>sudo</b> - The <b>sudo</b> command is used to ensure that the command runs with root access.
>>> - <b>update</b> - the <b>update</b> option is used ensure that all packages are updated on the Linux system.
>> ### Return Value
>> None
>> ### Example
>> ```
>> sudo apt-get update
>>```
>> ### Output
>> When we run the above command, we will get the following result
>> ![command of sudo apt-get update](/TutorialsPoint/res/img/example_output.jpg)
>>
>> This command will connect to the internet and download the latest system packages for Ubuntu.
> ## Step 3.
> The next step is to install the necessary certificates that will be required to work with the Docker site later on to download the necessary Docker packages. It can be done with the following command.
>>```
>> sudo apt-get install apt-transport-https ca-certificates
>>```
>> ![necessary docker packages](/TutorialsPoint/res/img/necessary_docker_packages.jpg)
> ## Step 4.
> The next step is to add the new GPG key. This key is required to ensure that all data is encrypted when downloading the necessary packages for Docker.
> The following command will download the key with the ID 58118E89F3A912897C070ADBF76221572C52609D from the <b>keyserver</b> hkp://ha.pool.sks-keyservers.net:80 and adds it to the <b>adv</b> keychain. Please note that this particular key is required to download the necessary Docker packages.
![new pgp key](/TutorialsPoint/res/img/new_pgp_key.jpg)
> ## Step 5.
> Next, depending on the version of Ubuntu you have, you will need to add the nelevant site to the <b>docker.list</b> for the <b>apt package manager</b>, so that it will be able to detect the Docker packages from the Docker site and download them accordingly.
>> - Precise 12.04 (LTS) - deb https://apt.dockerproject.org/repo ubuntu-precise main
>> - Trusty 14.04 (LTS) - deb https://apt.dockerproject.org/repo/ ubuntu-trusty main
>> - wily 15.10 - deb https://apt.dockerproject.org/repo ubuntu-wily main
>> - Xenial 16.04 (LTS) - https://apt-dockerproject.org/repo ubuntu-xenial main
>>
>> Since our OS is Ubuntu 14.04, we will use the Repository name as "deb https://apt.dockerproject.org/repo ubuntu-trusty main".
>>
>> And then, we will need to add this repository to the <b>docker.list</b> as mentioned above.
>> ```
>> echo "deb https://dockerproject.org/repo ubuntu-trusty main"
>>     | sudo tee /etc/apt/sources.list.d/docker.list
>>```
>> ![docker list](/TutorialsPoint/res/img/docker_list.jpg)
> ## Step 6
> Next, 


