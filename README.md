# rpi-mongo

This repository contains Dockerfile of [MongoDB](http://www.mongodb.org/) for [Raspberry Pi](https://www.raspberrypi.org/) published to the public [Docker Hub](https://hub.docker.com/r/azcoigreach/).

### Base Docker Image

* [resin/rpi-raspbian:jessie](https://github.com/resin-io-library/resin-rpi-raspbian)

### Installation

1. Install [Docker for Raspberry Pi](http://blog.hypriot.com/).

2. Download from [Docker Hub](https://hub.docker.com/u/azcoigreach/):

    `docker pull azcoigreach/rpi-mongo`

3. Alternatively, you can build an image from Dockerfile (**In you Raspberry Pi**):

    1. Update the proxy settings for apt-get in `10proxy`.

    2. `docker build -t="azcoigreach/rpi-mongo" github.com/azcoigreach/rpi-mongo`

### Usage

1. Run `mongod`:

    `docker run -it -p 27017:27017 --name mongodb azcoigreach/rpi-mongo`

2. For more usage details, please refer to [mongo](https://hub.docker.com/_/mongo/).