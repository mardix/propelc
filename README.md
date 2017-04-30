
# PROPELC

PropelC is a python deployment tool using Ansible on the client side, and Propel on the Server.
Hence 'C' is for Client in PropelC.


### Install on the client

    pip install propelc

### Setup

PropelC requires that you have `propel.yml` at the root of your application.

### To setup if you already have a propel.yml file

    propelc --init

### To setup if you don't have propel.yml file yet. It will create it.

    propelc --init --mkfile



## Usage

Once setup, you can run the following commands to provision your server and deploy to them

### --provision

Provision will setup all the servers with `propel` and create your application directory where the files
will reside at. This is done with `Propel`

    propelc --provision


### --deploy | -a [containers...] or --all | -a

Once your servers have been provisioned, you can deploy your containers.

A container is a set of command that will be eecuted on a host

    propelc -d containerA containerB containerC

    propelc -a


### --list

To show all the containers you have



