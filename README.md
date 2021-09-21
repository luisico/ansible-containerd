Containerd
==========
Install containerd CRI.

Container is installed from packages available in Docker's CE Stable package repository. For Centos, the `centos-extra` repository must be enabled. For Red Hat, `centos-extra` needs to be also added, including Centos GPG key. These dependencies are not included in this role. The latest version of containerd found in the repository is installed unless it is overridden with `container_version`.

Recommended setup that should be done outside of this role:
  - Install `centos-extra` repo.

Requirements
------------
See `meta/main.yml`.

Role Variables
--------------
See `defaults/main.yml`.

Dependencies
------------
`centos-extra` repository is needed for CentOS and Red Hat (see above).

Example Playbook
----------------
Example:
```
- hosts: servers
  roles:
    - containerd
```

TODO
----

License
-------

Author Information
------------------
Luis Gracia while at [Rockefeller University](http://www.rockefeller.edu):
- lgracia [at] rockefeller.edu
- GitHub at [luisico](https://github.com/luisico)
- Galaxy at [luisico](https://galaxy.ansible.com/luisico)
