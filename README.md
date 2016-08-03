Test environment for Spark
==========================

A virtual machine with Spark and Jupyter installed

## Pre-requisites

 * VirtualBox www.virtualbox.org
 * Vagrant www.vagrantup.com

## Using the VM

Vagrant manages the virtual machine, downloading a base image and installing
Spark and Jupyter. Any files in this directory are available on the virtual
macine at `/vagrant`, this is also the default location for Jupyter

### Start

    vagrant up

You can then go to `http://localhost8880` on the host machine to access Jupyter,
or `vagrant ssh` to log into the VM and run `/opt/spark/bin/pyspark`

### Stop

    vagrant destroy

