# ansible-demo
Small repository learning to use Ansible and the Ansible-Playbook technology to deploy a small AWS stack consisting of two EC2 instances and an ELB. This is connected to provide a simple HTML5 application, backed by an nginx server behind an ELB.  

## Pre-requisites

## Running
 - Ensure you have Python 2.5+ and easy_install
 - `sudo easy_install pip`
 - `sudo pip install ansible`
 - In `/etc/ansible/hosts` put `localhost ansible_connection=local
 - Install the human_log.py via [cliffano](https://gist.github.com/cliffano/9868180) at `/etc/ansible/plugins/logging/human_log.py`
 - Your local machine must have `aws-cli` installed and setup with keys to your AWS account
 - Run `ansible-playbook chuck-demo.yml` and away you go!
