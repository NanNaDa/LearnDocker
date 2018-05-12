# Installing Docker on Linux
To start the installation of Docker, we are going to use an Ubuntu instance. You can use Oracle Virtual Box to setup a virtual Linux instance, in case you don't have it already.

The following screenshot shows a simple Ubuntu server which has been installed on Oracle Virtual Box. There is an OS user named <b>demo</b> which has been defined on the system having entire root access to the server.

![a picture of demo example](/TutorialsPoint/res/img/demo_button.jpg)

To install Docker, we need to follow the steps given below.

> ## Step 1. - Before installing Docker, you first have to ensure that you have the right Linux kernel version running. Docker is only designed to run on Linux kernel version 3.8 and higher. We can do this by running the following command.
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
> ## Step 2. - You need to update the OS with the latest packages, which can be done via the following command
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
>> This command will connect to the internet and download the latest system packages for Ubuntu.
> ## Step 3. -

