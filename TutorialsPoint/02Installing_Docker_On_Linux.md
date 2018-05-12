# Installing Docker on Linux
To start the installation of Docker, we are going to use an Ubuntu instance. You can use Oracle Virtual Box to setup a virtual Linux instance, in case you don't have it already.

The following screenshot shows a simple Ubuntu server which has been installed on Oracle Virtual Box. There is an OS user named <b>demo</b> which has been defined on the system having entire root access to the server.

![a picture of demo example](/TutorialsPoint/res/img/demo_button.jpg)

To install Docker, we need to follow the steps given below.

> Step 1. - Before installing Docker, you first have to ensure that you have the right Linux kernel version running. Docker is only designed to run on Linux kernel version 3.8 and higher. We can do this by running the following command.
>> <b>uname</b>
>> <p>This method returns the system informtion about the linux system.</p>
>>
>> <b> Syntax</b>
>> ```
>> uname -a
>> ```
