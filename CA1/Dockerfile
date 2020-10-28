#The FROM instruction initializes a new build stage and sets the Base Image for subsequent instructions. All valid Dockerfiles must begin with FROM
#It is easiest to pull an image from a the public repos.
#FROM can appear multiple times within a single Dockerfile to create multiple images or use one build stage as a dependency for another.
#Each FROM instruction clears any state created by previous instructions.
FROM python:3.9

#The COPY instruction copies new files or directories from source and adds them to the filesystem of the container at the path destination.
#Multiple source resources may be specified but the paths of files and directories will be interpreted as relative to the source of the context of the build.
#Dockerfile and DockerTutorial.html are in the same dir so source of the latter doesn't need to be specified.
COPY DockerTutorial.html /

#The EXPOSE instruction informs Docker that the container listens on the specified network ports at runtime.
#You can specify whether the port listens on TCP or UDP, and the default is TCP if the protocol is not specified.
EXPOSE 8080

#There can only be one CMD instruction in a Dockerfile. If you list more than one CMD then only the last CMD will take effect.

#The main purpose of a CMD is to provide defaults for an executing container. 
#These defaults can include an executable, or they can omit the executable.
CMD python3 -m http.server 8080
