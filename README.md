# docker-registry
Contains all code necessary to set up a private Docker Registry, and a Jenkins server to feed it

## Inspiration
- a DigitalOcean tutorial on [How To Set Up a Private Docker Registry on Ubuntu 14.04](https://www.digitalocean.com/community/tutorials/how-to-set-up-a-private-docker-registry-on-ubuntu-14-04)
- three Riot Games Engineering tutorials:
  - [Thinking inside the container](https://engineering.riotgames.com/news/thinking-inside-container)
  - [Putting Jenkins in a container](https://engineering.riotgames.com/news/putting-jenkins-docker-container)
  - [Docker & Jenkins: data that persist](https://engineering.riotgames.com/news/docker-jenkins-data-persists)

## Installation

    cd /
    sudo git clone https://github.com/fdurant/docker-registry.git
    sudo cp systemd-conf /lib/systemd/system
    sudo systemctl daemon-reload
    sudo service docker-registry start
