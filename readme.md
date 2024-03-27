# A lightweight docker image for running windows applications in a container

## Usage
This image is intended as a base image providing the basics to running a GUI windows application on docker.

### Standalone
If this image is run without any additional arguments, it launches the VNC server and dwm.

### As parent image
If this image is used as a base image, in the child-dockerfile, pass your own arguments using `CMD [ "<your args>" ]`. 
They will get executed after the container started up (X server and dwm)
