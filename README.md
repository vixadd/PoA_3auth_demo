# 3-Authority PoA Network
## Introduction
### Demo
This is a demo to demonstrate the capabilities of a PoA Network. It is set up and deployed using docker-compose.
Therefor, you need to make sure you have docker-compose installed.
```bash
$ sudo apt-get install docker-compose
```
Setting up Parity Ethereum is a must.
```bash
$ sudo apt-get install build-essential openssl libssl-dev libudev-dev
$ bash <(curl https://get.parity.io -L)
```
### Deployment and Monitoring
Occures with a foundation of the etstat dashboard. Pm2 is also a component on the docker build.
To deploy the application the docker-compose config needs to be activated.
After installing both docker and docker-compose run the following command.
```bash
$ sudo docker-compose up
```
This will allow you to set up the core foundation of the demo network. After running it you can run the docker-compose script in the background with:
```bash
$ sudo docker-compose up -d
```
