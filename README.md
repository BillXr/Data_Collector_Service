# Data-Collector-Service
Collect data from different hosts in the cloud.

This project was created for the class "Cloud Computing and Services" in university.
The main purpose of project was to create a container(swarm) of virtual machines and make them communicate with each other in different ways.

## Steps

+ Network creation

  * Automatic installation of a program for data collection

  * onEvent - local / temporary data storage

----------------------------------------------------------
+ Database replication

  * onEvent data storage in the database

----------------------------------------------------------
+ Create GUI or

  * Create a Websocket connection to the database or basic services for instant data transfer

-----------------------------------------------------------
## Stack

+ Fluentd

+ Ansible

+ Swarmlab

+ MongoDB

+ NodeJS

----------------------------------------------------------
## Execution

+ First of all fluentd.yml install fluentd tool in all hosts.

+ After that fluentd.yml.sh searches for ip addresses and when he finds them,runs ansible script in all swarm.

+ Additionally fluentd-config-update file write all the logs we have in database.

+ In addition fluentd.-config-update.yml.sh refreshes all ip addresses we have found,and runs ansible script in swarm.

+ Finally we write down all ip addresses of swarm.


