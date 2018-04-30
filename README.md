# Deploying VoltDB to a DC/OS Cluster

## Overview
VoltDB is an in-memory database available for application modernization initiaves and also as an in-memory repository to improve performance of legacy stores.  This posting covers the steps to gain the performance benefits of VoltDB along with the modern platform benefits of Mesosphere DC/OS.
 

## Requirements
The instructions in this README cover the open source version of VoltDB.  Though the VoltDB enterprise version should also work with only a change to the Docker Image referenced.

The general requirements for this process include:
* A DC/OS cluster running 1.10+
* Access to the open source VoltDB docker image via the same servers as which constitute the DC/OS cluster.

## Installation Steps
1. type 'dcos marathon app add '
## Validating the Installation