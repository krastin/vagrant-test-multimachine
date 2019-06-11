# vagrant-test-multimachine
A multimachine vagrant file containing two web servers and a database server

# List of machines

- web01

- web02

- mysql

# VM Image used

[Ubuntu Xenial 64](https://app.vagrantup.com/krastin/boxes/xenial64)

# How to Use

## Install Vagrant
Learn where to grab Vagrant from and how to install it [here](https://www.vagrantup.com/docs/installation/).

## Create machine instances
   
    vagrant up
   
First time it will take a while because the VM image is being downloaded

## Log on to machine instances

Usernames and/or passwords, where applicable, are either _ubuntu_ or just nothing.

    vagrant ssh web01
    vagrant ssh web02
    vagrant ssh mysql
    
## Destroy machine instances

    vagrant destroy -f

# TODO

Not much

# DONE

- [x] Add Vagrantfile
- [x] Add Install Vagrant documentation
- [x] Add Create Machines documentation
