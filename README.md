# ansible-cloudera-hadoop-stack

This contains a role hdfs-cdh, which can be used to installs cloudera distribution of Hadoop. BUT, IT DOESN'T SETUP CLOUDERA MANAGER. This role installs:

* java (optionally)
* snakebite (optionally) - python HDFS client that uses protobuf for communicating with the NameNode and comes in the form of a library and a command line interface (https://github.com/spotify/snakebite)
* selected cdh packages

## Tested platforms:
Tested with python 2.7 in the following platforms
* Ubuntu 14.04
* Ubuntu 16.04

## Usage: 
   * download the repository
   * _cd ansible-cloudera-hadoop-stack_
   * modify files under _inventory/local/_ based on your environment
   * modify _install-hdfs-client-nodes.yml_ for your own package selection per node and node type
   * execute _ansible-playbook -i inventory/local install-hdfs-client-nodes.yml_
