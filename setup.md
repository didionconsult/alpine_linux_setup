== Basic Setup ==



// Determine Docker container name and get shell access to it
$ docker ps
$ docker exec -it <container_name> sh

// Update your current package list
$ apk update

// identify user
whoami

/ install bash and switch current shell to bash
$ apk add bash
$ bash --version
$ bash

// Install curl 
$ apk add curl
$ curl --version

// Install wget
$ apk add wget
$ wget --version

// Install vim 
$ apk add vim
$ vi --version

// Install nano
$ apk add nano
$ nano --version

// Install mlocate
$ apk add mlocate
locate --version

// Use updatedb to create a database for mlocate 
updatedb

// Add any other package
$ apk add <package_name>

// Search more packages
$ apk search -v 'node'

// Rename image
$ docker rename my_container my_new_container

// Stop and quit
$ docker stop <image_name>

