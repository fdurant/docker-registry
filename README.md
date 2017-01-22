# docker-registry
Contains all code necessary to set up a private Docker Registry

Inspired by this excellent [DigitalOcean tutorial](https://www.digitalocean.com/community/tutorials/how-to-set-up-a-private-docker-registry-on-ubuntu-14-04)

## Installation

cd /
sudo git clone https://github.com/fdurant/docker-registry.git
sudo cp systemd-conf /lib/systemd/system
sudo systemctl daemon-reload
sudo service docker-registry start
