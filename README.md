# docker-arm-gcc
A docker container  with arm gcc toolchain for gcc


arm gcc toolchain download from https://launchpad.net/gcc-arm-embedded


```bash

usage () {
  echo "Usage: launcher.sh COMMAND"
  echo "Commands:"
  echo "    start:      Start/initialize a container"
  echo "    stop:       Stop a running container"
  echo "    restart:    Restart a container"
  echo "    destroy:    Stop and remove a container"
  echo "    enter:      Use nsenter to enter a container"
  echo "    ssh:        Start a bash shell in a running container"
  echo "    build:      Build a new container "
  echo "    rebuild:    Rebuild a container (destroy old, bootstrap, start new)"
  echo "    cleanup:    Remove all containers that have stopped for > 24 hours"
  echo
  exit 1
}

```


# Licenese:
MIT.See LICENSE file.

