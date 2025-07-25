- Project decriptions

- ssh connection between two servers.

- Using the ssh client server in this project.

- Some points to learn this project
    - Improved security
    - Ease of management
    - Better collaboration 
    - Scalability
    - Portability

- How to install the ubuntu or centos 
    - docker pull ubuntu
    - docker pull centos

- How to run the docker container in cmd?
    docker run -it --name container1 ubuntu

- update the container in using the command apt-get update.
- install the openssh-server in the images.
    apt-get install openssh-server

- install the text editor in this images.
    apt-get install nano

- Go to ssh main file path and edit the ssh server file.
    nano /etc/ssh/sshd_config

- edit the Authentication sections - PermitRootLogin yes type.

- check the service status in the ubuntu - services --status-all
- start the ssh service - services ssh start.

- create the second conatiner, update the ubuntu images file, install the openssh-client and also install vim text editor.
- apt-get install openssh-client, apt-get install vim.

- start the container1
    - docker start container1
    - login into the container 1 
        -   docker exec -it container1 bash
    - check the docker container ip address docker inspect container1 | grep IPAddress

- start the container2
    - docker start container1
    - login into the container 1 
        -   docker exec -it container1 bash
    - check the docker container ip address docker inspect container1 | grep IPAddress
    
- to connect the main server to client server.
    - cmd- ssh root@ip_address 
