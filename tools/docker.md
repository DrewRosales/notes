Build docker image based on DockerFile
`docker build -t [repository:tag][DockerFile-directory]`

List docker images
`docker image ls`

Delete images
`docker image rm -f [image-name]`

Run container in interactive
`docker run -it [image-name]`

Run docker in detached mode
`docker run -d --name [container-name][image-name]`

## Docker Compose
Docker compose can be used to manage the network,internal processes, and more based on a YAML file

Begin the Docker Compose in working directory with compose YAML file
`docker compose up`
