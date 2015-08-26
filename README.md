# ansible-demo
Small repository learning to use Ansible and the Ansible-Playbook technology to deploy a small AWS stack consisting of a single EC2 instance and an ELB. This is connected to provide a simple HTML5 application, served by nginx. Ansible will run on your localhost and remotely deploy and configure the stack for you!  

Tested to work on OSX systems.  

## Pre-requisites
 - Python 2.6+
 - ansible installed on localhost using easy_install

## Running
 - In `/etc/ansible/hosts` put `localhost ansible_connection=local`
 - Your local machine must have `aws-cli` installed and setup with keys to your AWS account responding with JSON
 - Configure the vars in `chuck-demo.yml` to your liking (keys, names etc)
 - Run `ansible-playbook chuck-demo.yml` and away you go!

## Optional 
 - Install the human_log.py via [cliffano](https://gist.github.com/cliffano/9868180) at `/etc/ansible/plugins/logging/human_log.py` to see stdout, stderr etc...
