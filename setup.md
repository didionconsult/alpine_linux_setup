== Basic Provisioning for an Alpine Linux Server ==


// Determine Docker container name and get shell access to it
```sh
$ docker ps
$ docker exec -it <container_name> sh
```

// Update your current package list
```sh
$ apk update
```

// identify user
```sh
whoami
```

// install bash and switch current shell to bash
```sh
$ apk add bash
$ bash --version
$ bash
```

// Install curl 
```sh
$ apk add curl
$ curl --version
```sh

// Install wget
```sh
$ apk add wget
$ wget --version
```

// Install vim
```sh
$ apk add vim
$ vi --version
```
or

// Install nano
```sh
$ apk add nano
$ nano --version
```

// Install mlocate
```sh
$ apk add mlocate
locate --version
```
// Create locate database 
```sh
updatedb
```

// Search more packages
```sh
$ apk search -v 'node'
```

// Rename image (if needed)
```sh
$ docker rename my_container my_new_container
```

// Stop container
```sh
$ docker stop <image_name>
```
