# Helpful tips I probably wont rememember
-- Under Construction --

The docker files in the repo - may not be consistent with the commands below, but have been included just to see the format

### Build from docker file
`docker run --rm -it repronim/neurodocker:latest generate docker --pkg-manager apt --base-image ubuntu:22.04 --entrypoint /bin/bash --freesurfer version=7.3.1 > ~/repo/Dockerfiles/ubuntu22.04_freesurfer7.3.1_bash` <br><br>
`podman build -f ./---.Dockerfile` <br>

### Sections of dockerfile
```
FROM debian:buster-slim
ENV OS="Linux" \   
   ....
RUN
ENTRYPOINT
...
````




`podman image list`
`podman container list`

### Get a bash terminal to run freesurfer commands
`podman run --rm -it localhost/freesurfer:latest bash`


```
docker run --detach --name my_container -it ubuntu:latest
docker exec -it my_container bash
```

If bash does not run - may need to add flags to entrypoint <br>
https://stackoverflow.com/questions/61055324/docker-cannot-execute-binary-file

Docker/Podman with github actions: <br>
https://dev.to/mihinduranasinghe/using-docker-containers-in-jobs-github-actions-3eof

Running jobs in docker container on github actions: <br>
https://docs.github.com/en/actions/using-jobs/running-jobs-in-a-container

