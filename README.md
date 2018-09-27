# ptdefender-docker

Profit Trailer Defender Docker

Compatible with Profit Trailer Defender version : v1.11.3

Wiki `https://github.com/PTDefender/Welcome/wiki`

## Install Docker

- Windows `https://docs.docker.com/toolbox/toolbox_install_windows/`
- Mac OS `https://docs.docker.com/docker-for-mac/install/`
- Linux Ubuntu `https://docs.docker.com/install/linux/docker-ce/ubuntu/#install-docker-ce`

## Quick Guide

### Run latest Profit Trailer Defender version

- To Run Container and replace `<your path>` with the full path where your profit trailer application.properties file is.

```bash
docker run -v <your path>/application.properties:/home/headless/ProfitTrailer/application.properties -p 6901:6901 -p 5901:5901 --name ptdefender jakkie/ptdefender-docker
```

- After Profit Trailer is running browse to the url example `http://your-ip:6901`
- Default vnc password is headless
- Once login to vnc the ptdefender app icon should be on the desktop.

### Running Profit Trailer Defender with docker-compose

- To install docker compose see `https://docs.docker.com/compose/install/`
- Edit your docker-compose file to include the volume where your profit traler installation is.
- To start docker-compose to run the container.

```bash
docker-compose up -d