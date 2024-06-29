# cd to this dir
* docker build . -t ansible
* docker run -d -v ~/VSC-Projects/ansible/yt-jim-ansible:/etc/ansible --name ansible ansible # -d means deathed mode the last paramter is always the name of the docker image we want to run , -v attach a volume from our host to the remote host we use /etc/ansible becuase thats what we specified as CMD in the Dockerfile
* docker exec -it ansible /bin/bash # ansible the name of the container we want to connect to -it = interactive and /bin/bash is the app we want to run when we connect to the image