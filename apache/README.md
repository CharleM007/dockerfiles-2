# Readme

This builds an Docker image with apache from using the amazonlinux:2 image as a base.

It installs some common commands to help with debugging and useful for this tutorial: [Docker Introduction Tutorial](https://blog.boltops.com/2018/04/19/docker-introduction-tutorial)

## Build

    docker build -t apache:tutorial .

## Run

    docker run apache:tutorial
