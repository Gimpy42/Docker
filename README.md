# Pen testing tool on docker
Various Dockerfile for pen testing tool,

This project was made to simplified and unified tool in a team across different os

## LinkedInt
Build the container:

`docker build -t linkedint .`

Complete the config file and start the container:

```docker run --rm -it --mount type=bind,source=/PATH/TO/LinkedInt.cfg,target=/LinkedInt/LinkedInt.cfg -v `pwd`:/data linkedint```

## Sublist3r
Build the container:

`docker build -t sublist3r .`

Start the container:

```docker run --rm -it -v `pwd`:/data sublist3r```

