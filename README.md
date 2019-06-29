# data_science_tools

### Install redis-server

```shell
sudo apt-get install redis-server
sudo systemctl enable redis-server.service
redis-cli

```

### Install Casandra

```shell
sudo apt install openjdk-11-jdk
echo "deb http://www.apache.org/dist/cassandra/debian 39x main" | sudo tee -a /etc/apt/sources.list.d/cassandra.sources.list
sudo apt install curl
curl https://www.apache.org/dist/cassandra/KEYS | sudo apt-key add -
sudo apt update
cqlsh
```

### Install MongoDB

```shell
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 68818C72E52529D4
sudo echo "deb http://repo.mongodb.org/apt/ubuntu bionic/mongodb-org/4.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-4.0.list
sudo apt-get update
sudo apt-get install -y mongodb-org
sudo systemctl start mongod
sudo systemctl enable mongod
mongo
```