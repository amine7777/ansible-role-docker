Ansible role: Docker
=========

This role helps you to install docker on your linux machine.


|Travis|CircleCI|GitHub|Quality|Downloads|Version|
|------|--------|------|-------|---------|-------|
|[![travis](https://travis-ci.com/amine7777/ansible-role-docker.svg?branch=master)](https://travis-ci.com/amine7777/ansible-role-docker)|![circleci](https://circleci.com/gh/amine7777/ansible-role-docker.svg?style=svg)|[![github](https://github.com/amine7777/ansible-role-docker/workflows/CI/badge.svg)](https://github.com/amine7777/ansible-role-docker/actions)|[![quality](https://img.shields.io/ansible/quality/50498)](https://galaxy.ansible.com/amine7777/docker)|[![downloads](https://img.shields.io/ansible/role/d/50348)](https://galaxy.ansible.com/amine7777/docker)|[![Version](https://img.shields.io/github/release/amine7777/ansible-role-docker.svg)](https://github.com/amine7777/ansible-role-docker/releases/)|

![](docker.jpg)

Requirements
------------
- Linux machine
- Ansible 2.9

Role Variables
--------------
These variables helps to manage docker installation.

You can specify your docker version in this variable.
```yaml
docker_version: 0.13.1
docker_arch: amd64
docker_directory_path: /usr/local/bin
```
This is the url where docker will be downloaded.
```ỳaml
docker_download_url: 'https://releases.hashicorp.com/docker/{{ docker_version }}/docker_{{ docker_version }}_linux_{{ docker_arch }}.zip'
```
This is the path where packer binary will be stored.
```yaml
docker_directory_path: /usr/local/bin
```

Example Playbook
----------------

```yaml
- hosts: all
  roles:
     - amine7777.docker
```


Author Information
------------------

- [Amine Kahlaoui](https://github.com/amine7777), DevOps engineer.
