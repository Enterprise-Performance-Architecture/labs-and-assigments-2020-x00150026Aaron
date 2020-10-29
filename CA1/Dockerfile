#This is the first command in a Dockerfile and is needed to run properly.
#This command is used to format a new build stage and indicates what base image to use for the following instructions.
#You can use local images or pull one from public repos. FROM can be used multiple times to create several images.
FROM python:3.9

#This sets the work directory to CA1. Commands such as RUN, CMD and COPY are to be executed here.
WORKDIR /CA1

#This command copies files or whole directories from a sepcified local source to a specified destination within the container.
#Several source files or directories can be copied in the one command. The location of these files are interpreted as relative to the directory you are building the docker in.
#Dockerfile and DockerTutorial.html are in the same dir, so source of the latter doesn't need to be specified.
COPY DockerTutorial.html /CA1

#Only one CMD command is needed for a Dockerfile, if you use more than one only the last one will work.
#CMD is used to provide defaults for an executing container such as including or omiting an executable.
CMD python3 -m http.server 8080
