Ansible Role: podman
=========

Archiving this role as podman now ships with most major distributions, no role needed.

[![CI](https://github.com/guidugli/ansible-role-podman/workflows/CI/badge.svg?event=push)](https://github.com/guidugli/ansible-role-podman/actions?query=workflow%3ACI)

An Ansible Role that install and configure podman on RHEL/CentOS, Fedora and Debian/Ubuntu. The focus is the installation on distributions that ships it in its repository. For a more comprehensive role, use [this one](https://github.com/alvistack/ansible-role-podman)

Requirements
------------

No requirements.

Role Variables
--------------

**Available variables are listed below, along with default values (see defaults/main.yml):**

    #podman_max_user_namespaces: 28633

Increase the number of user namespaces in the kernel
Reference: [Set up for rootless containers](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux_atomic_host/7/html-single/managing_containers/index#set_up_for_rootless_containers)

**The variables listed below do not need to be changed for targeted systems (see vars/main.yml):**

    podman_packages:

Provides a list of packages to be installed based on operating system and version.

Dependencies
------------

No dependencies.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: guidugli.podman }

License
-------

MIT / BSD

Author Information
------------------

This role was created in 2020 by Carlos Guidugli.
