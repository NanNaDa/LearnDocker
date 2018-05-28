# Architecture
The following image shows the standard and traditional architecture of **virtualization**.

![Virtualization](/TutorialsPoint/res/img/virtualization.jpg)

- The server is the physical server that is used to host multiple virtual machines.
- The Host OS is the base machine such as Linux or Windows.
- The Hypervisor is either VMWare or Windows Hyper V that is used to host virtual machines.
- You would then install multiple operating systems as virtual machines on top of the existing hypervisor as Guest OS.
- You would then host your applications on top of each Guest OS.

The following image shows the new generation of virtualization that is enabled via Dockers.
Let's have a look at the various layers.

![Various Layers](/TutorialsPoint/res/img/various_layers.jpg)

- The server is the physical server that is used to host multiple virtual machines. So this layer remains the same.
- The Host OS is the base machine such as Linux or Windows. So this layer remains the same.
- Now comes the new generation which is Docker engine. This is used to run the operating system which earlier used to be virtual machines as Docker containers.
- All of the Apps now run as Docker containers.

The clear advantage in this architecture is that you don't need to have extra hardware for Guest OS. Everything works as Docker containers.

