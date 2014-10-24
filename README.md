MONO Dockerfile

This repository contains Dockerfile of MONO for Docker's automated build published to the public Docker Hub Registry.
Base Docker Image

    dockerfile/debian

Mono is installed using the Apt repo published by xamarin "deb http://download.mono-project.com/repo/debian wheezy main" which has the latest mono version at the time this container is built. Older versions can be used by using the specific tag for that version. Older version are installed by using the snapshot repository of that specific repository.

* Install Docker.

* Download automated build from public Docker Hub Registry:
    docker pull seif/mono

Usage

    docker run -it --rm seif/mono mono
