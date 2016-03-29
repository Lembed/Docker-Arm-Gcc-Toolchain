# docker-arm-gcc
A docker container  with arm gcc toolchain for gcc


arm gcc toolchain download from https://launchpad.net/gcc-arm-embedded


```bash
# build the image
docker build --tag image-gccarm:v0.01 .

# ceate a container, adjust --volume args
docker create \
    --name arm-gcc-embedded \
    --publish 8022:22 \
    --volume /home/gaembed/workspace/:/home/gaembed/workspace \
    image-gaembed:v0.01

# start the container
docker start arm-gcc-embedded

# ssh into it
ssh -p 8022 gaembed@localhost

# stop the container
docker stop arm-gcc-embedded

# delete the container and image, if you don't need these anymore
docker rm arm-gcc-embedded
docker rmi image-gaembed:v0.01
```


# Licenese:
MIT.See LICENSE file.

