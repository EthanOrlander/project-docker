# project-docker
Docker file for developing the course project.

1. First, download Docker and go through the initial set-up on their website.

2. Clone the course project repository, then open terminal and cd into it.

3. Once in the folder with the Dockerfile use the command:

docker run -t -i -v localDirectory:containerDirectory ubuntu /bin/bash

localDirectory is the folder on your computer you want to connect to the docker container

containerDirectory is the name of the folder in the container you want to tie to your local directory. If the folder does not exist the container will automatically create it.

4. From there the two folders should be connected, everything you do in one automatically updates in the other. For the project you will write the code in your local directory and then run it through the docker command line. A quick test to see if they're working is to create a file in the folder on your computer then use the terminal to see if it also shows up in the docker container.