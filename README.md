# Deploying VoltDB to a DC/OS Cluster

## Overview
VoltDB is an in-memory database available for application modernization initiaves and also as an in-memory repository to improve performance of legacy stores.  This posting covers the steps to gain the performance benefits of VoltDB along with the modern platform benefits of Mesosphere DC/OS.
 

## Requirements
The instructions in this README cover the open source version of VoltDB.  Though the VoltDB enterprise version should also work with only a change to the Docker Image referenced.

The general requirements for this process include:
* A DC/OS cluster running 1.10+
* Access to the open source VoltDB docker image via the same servers as which constitute the DC/OS cluster.

## Installation Steps
1. Define the node attribute 'voltdb' and give it the value 'true' for the 3 nodes you wish to deploy VoltDB.  You can have more than 3 nodes, but if you do then you will need to update the 'voltdb-bridge.json' to have the number of nodes desired.
2. Add the voltdb container to Marathon by executing the following commands:
```
cd src/installation
dcos marathon app add voltdb-host.json
```
