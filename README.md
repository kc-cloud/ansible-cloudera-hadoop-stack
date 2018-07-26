# ansible-cloudera-hadoop-stack

** This contains a role hdfs-cdh, which can be used to install Cloudera Hadoop ecosystem in name nodes, worker nodes and edge nodes

Currently this works on Ubuntu based linux systems.  Tested platforms are:

* Ubuntu 14.04/16.04

## Usage

** Download the repository

** Use the following files to configure your nodes:

* /inventory/local/hosts

** Use Ansible the following playbooks to install the hadoop in your respective node groups

* install-hdfs-client-nodes.yml
* install-hdfs-name-nodes.yml
* install-hdfs-worker-nodes.yml

