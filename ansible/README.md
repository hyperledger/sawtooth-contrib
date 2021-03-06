Sawtooth-ansible

This repository provides a set of generic Ansible roles that can be
used as building blocks for creating a Hyperledger Sawtooth network.

1) Modify the hosts file to match the network, host names, and IP addresses of
the environment. See hosts-example to get started.

2) Create a configuration yaml file based off the config-example.yaml. Here
you can modify several parameters used for installation, and configuration.

3) Create playbooks to put the roles together. A couple playbooks are provided
showing ways these roles can be used.

Usage
`ansible-playbook -i hosts --extra-vars "@./configs/config.yaml" -f 2 sawtooth-deploy.yaml`
