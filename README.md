# dockerMadeEasy
simple docker container that has a webpage on boot



# First install Docker (ubuntu instructions)

If you want to run Docker without using Docker Desktop, you can install Docker Engine directly on your system. This is commonly done on Linux systems where Docker can be managed entirely via the command line. Below are the steps for installing Docker Engine on various operating systems:

### Linux
For most Linux distributions, Docker can be installed directly from the official repositories or Docker’s repositories. Here’s how you can install it on some of the most popular Linux distributions:

#### Ubuntu
1. Update your package index:
   ```bash
   sudo apt update
   ```
2. Install the necessary packages to allow `apt` to use a repository over HTTPS:
   ```bash
   sudo apt install apt-transport-https ca-certificates curl software-properties-common
   ```
3. Add Docker’s official GPG key:
   ```bash
   curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
   ```
4. Set up the stable repository:
   ```bash
   sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
   ```
5. Update the package database with the Docker packages from the newly added repo:
   ```bash
   sudo apt update
   ```
6. Install Docker CE (Community Edition):
   ```bash
   sudo apt install docker-ce
   ```
