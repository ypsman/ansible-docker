ansible docker
==============
[![Build Status](https://travis-ci.org/ypsman/ansible-docker.svg?branch=master)](https://travis-ci.org/ypsman/ansible-docker)

This Role installs Docker on your Debian/Ubuntu Server.

Import the gpg Key for the Repository.

Optional:

- Add a User to docker group.
- Specifie a docker-version to install and apt-pin it.

Example Playbook
----------------

    - hosts: all
      roles:
        - role: ypsman.docker
          docker_version: "1.12.1"  # optional
          docker_user: LinuxUser
