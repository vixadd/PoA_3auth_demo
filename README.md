# 3-Authority PoA Network
### Demo
This is a demo to analyze the capabilities of a PoA Network. It is set up and deployed using docker-compose.
Therefor, you need to make sure you have docker-compose and docker installed.
```bash
$ sudo apt-get install docker
$ sudo apt-get install docker-compose
```
Setting up Parity Ethereum is a must. Install the following required dependencies
```bash
$ sudo apt-get install build-essential openssl libssl-dev libudev-dev
$ bash <(curl https://get.parity.io -L)
```
### Deployment and Monitoring
Occures with the ethstat dashboard. PM2 is also a component on the build.
To deploy the application the docker-compose config needs to be activated.
After installing all required dependencies, run the following command.
```bash
$ sudo docker-compose up
```
This will allow you to set up the core foundation of the demo network. After running it you can run the docker-compose script in the background with:
```bash
$ sudo docker-compose up -d
```
This instruction initiates a dashboard and monitoring sequence using docker compose. At the same time it allows for the use of PM2 to monitor System Resource Usage.
Inorder to see the output of this monitor run the following command in the root directory of the repository.
```bash
$ sudo docker-compose logs monitor
```
You can add extra users on top of the current authorities by making user config files and running them.
#### RPC Interface
You can interact with this network over the central rpc interface to add more authorities and users.
You can make use of this interface over: <b>http://127.0.0.1:8545</b>
With this you can successfully pair authorities and users to one another through their enode adresses.
I added a single user into the e-authority network to lay a framework for everything.

