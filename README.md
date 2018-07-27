# ansible-cloudera-hadoop-stack

This contains a role hdfs-cdh, which can be used to install Cloudera Hadoop ecosystem. This role installs:

* java (optionally)
* snakebite (optionally) - python HDFS client that uses protobuf for communicating with the NameNode and comes in the form of a library and a command line interface (https://github.com/spotify/snakebite)
* selected cdh packages

## Tested platforms:
Tested with python 2.7 in the following platforms
* Ubuntu 14.04
* Ubuntu 16.04

## Usage: 
   * download the repository
   * cd ansible-cloudera-hadoop-stack
   * modify files under inventory/local/ based on your environment
   * modify install-hdfs-client-nodes.yml for your own package selection per node and node type
   * execute _ansible-playbook -i inventory/local install-hdfs-client-nodes.yml_
