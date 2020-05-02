
I have created a project on Docker, based on the concepts learnt from World Record holder Vimal Daga's Docker Training.

REQUIREMENTS:
           ORACLE VIRTUAL BOX
           BASE OPERATING SYSTEM: RED HAT ENTERPRISE LINUX (RHEL8)
           RAM: 4 GB
           STORAGE: 250GB
           CPU alloted in Virtual BOX: 2CPUs

Dockeris  a  system that  provides pre-configured, self-contained applications, frameworks, and software stacks, 
such as WordPress, Golang, or LAMP. Even entire Linux  distributions can  be run in  Docker. When deployed, 
these software packages are referred to as containers.  Docker also allows you to create your own containers that 
include any custom software.

ownCloud is a file sharing server that permits you to store your personal content, like documents and pictures, in a centralized location, much like Dropbox. 
The difference with ownCloud is that it is free and open-source, which allows anyone to use and examine it. 
It also returns the control and security of your sensitive data back to you, thus eliminating the utilization of a third-party cloud hosting service.

Docker Compose is a complementary system which helps you link together individual Docker containers so they can 
work together. 

PROJECT OBJECTIVE
------------------

Configuring Owncloud server with MySQL in Docker

PREREQUISITES:
-----------------

In order to complete the steps in this guide, you will need the following:

1. Root access to the OS.
2. YUM properly configured
3. Docker installed
4. MySQL image installed
5. Owncloud image installed


STEPS:
-------
1. Disable the firewall : systemctl stop firewalld 
2. Disable SELinux: setenforce 0
3. To see all docker images: docker images
4. Create new folder: mkdir myproject
                      cd myproject
5. Create a file named “docker-compose.yml” inside the “myproject” directory.
cd myproject
vim docker-compose.yml
6. Enter the source code
7. Run the docker-compose file: docker-compose up -d
8. Inpect the owncloud container using its container ID:
docker inspect [CONTAINER ID]
9. Get the IP address of owncloud container.
10. Open the URL in browser.
11. Proceed with the Owncloud installation steps and finish configuring the website.



