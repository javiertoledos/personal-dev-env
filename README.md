# Ansible local development

Playbook for replicating my local vm environment. 

## Motivation

I like testing new stuff. I wanted to learn ansible, and I'm working with virtualization. I have a Windows host and I prefer using a VM instead of WSL for development so I created this ansible to replicate my local development and to help other people to have an environment like mine.

## Installation

### Requirements
* Ansible locally instaled in the machine that will be self provisioned.
* Ubuntu 22.04. Non-debian distros are not tested and they won't likely work due lack of consideration.

## Usage

Run the following commands to provision your local:

```
ansible-galaxy install -r requirements.yml 
ansible-playbook playbook.yml
```

## Roadmap

* Parametrize ansible playbook so specific tools can be installed/excluded
* Add more programming languages I work with (and some I don't)
* Support different distros (mainly Fedora/Centos)
