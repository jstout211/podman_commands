# Helpful tips I probably wont rememember
-- Under Construction --

### Build from docker file
`docker run --rm -it repronim/neurodocker:latest generate docker --pkg-manager apt --base-image ubuntu:22.04 --entrypoint /bin/bash --freesurfer version=7.3.1 > ~/repo/Dockerfiles/ubuntu22.04_freesurfer7.3.1_bash` <br><br>
`podman build -f ./---.Dockerfile` <br>

### Sections of dockerfile
```
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
