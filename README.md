ansible docker
==============
[![Build Status](https://travis-ci.org/ypsman/ansible-docker.svg?branch=master)](https://travis-ci.org/ypsman/ansible-docker)

This Role installs Docker on your Server.

It imports the gpg Key for the Repository.

You can specifie a version to install and pin them.

The docker-version variable is optinal.

Example Playbook
----------------

    - hosts: all
      roles:
        - role: ypsman.docker
          docker_version: "1.12.1"  # optional
