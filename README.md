# docker-jenkins

Sets up a container with jenkins installed listening on port 8080.

## Usage

To run the container, do the following:

    docker run -d -P maxreiner/jenkins

    docker ps
    CONTAINER ID        IMAGE                       COMMAND                CREATED             STATUS              PORTS                     NAMES
    1131d37c38b1        maxreiner/jenkins:latest    java -jar /opt/jenki   12 seconds ago      Up 12 seconds       0.0.0.0:49153->8080/tcp   drunk_fermi

Your jenkins instance is now available by going to http://localhost:49153 .

By default, JENKINS_HOME is set to /jenkins.  

## Building

To build the image, simply invoke

    docker build github.com/maxreiner/docker-jenkins

A prebuilt container is also available in the docker index

    docker pull maxreiner/jenkins
