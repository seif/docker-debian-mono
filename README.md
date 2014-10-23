MONO Dockerfile

This repository contains Dockerfile of MONO for Docker's automated build published to the public Docker Hub Registry.
Base Docker Image

    dockerfile/debian

Mono is installed using the Apt repo publish by xamarin "deb http://download.mono-project.com/repo/debian wheezy main" which has the latest mono version at the time this container is built, still not sure how to handle locking to a specific version of mono, as the repository only has 1 version of mono at a time (latest stable).

Installation

    Install Docker.

    Download automated build from public Docker Hub Registry: docker pull seif/mono

Usage

docker run -it --rm seif/mono mono
