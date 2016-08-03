Test environment for Spark
==========================

A virtual machine with Spark and Jupyter/Ipython installed

## Pre-requisites

 * VirtualBox www.virtualbox.org
 * Vagrant www.vagrantup.com

## Using the VM

Vagrant manages the virtual machine, downloading a base image and installing
Spark and Jupyter. The repository directory is mounted on the virtual machine
as a shared directory, and is available at `/vagrant`. This is also the default
location for Jupyter, so notebooks created on the VM are saved when the VM is
shut down.

### Start

    vagrant up

You can then go to `localhost:8880` with a web browser on the host machine to
access Jupyter, or `vagrant ssh` to log into the VM and run
`/opt/spark/bin/pyspark` (or `spark-shell` for Scala)

### Stop

    vagrant destroy

## References

http://spark.apache.org/docs/latest/quick-start.html
http://www.cloudera.com/documentation/enterprise/5-5-x/topics/spark_ipython.html
