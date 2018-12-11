# Docker_tutorial

What Is Docker?

Docker describes themselves as "an open platform for developers and sysadmins to build, ship, and run distributed applications".

Docker allows you to run containers. A container is a sandboxed process running an application and its dependencies on the host operating system.
The application inside the container considers itself to be the only process running on the machine while the machine can run multiple containers independently.



Step1 ---> Installing docker on ubuntu

First, in order to ensure the downloads are valid, add the GPG key for the official Docker repository to your system:
$curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

Add the Docker repository to APT sources:
$sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"

Next, update the package database with the Docker packages from the newly added repo:
$sudo apt-get update

Make sure you are about to install from the Docker repo instead of the default Ubuntu repo:
$apt-cache policy docker-ce

Notice that docker-ce is not installed, but the candidate for installation is from the Docker repository for Ubuntu 16.04 (xenial).


Finally, install Docker:

$sudo apt-get install -y docker-ce

install docker successfully :)



Step2 ---> working with docker

For Show the Docker version information:
$docker --version

for example, output: Docker version 18.06.1-ce, build e68fc7a

where (18.06.1)the time is the commit time in UTC and (e68fc7a)the final suffix is the prefix of the commit hash and (ce) is docker version.

About  Docker CE

Docker Community Edition (CE) is ideal for developers and small teams looking to get started with Docker and experimenting with container-based apps.
