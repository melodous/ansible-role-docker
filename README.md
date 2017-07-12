Welcome to docker Ansible Role’s documentation!
===============================================

Role Name
---------

This role install docker engine on the server, and configure the
logging, monitoring and tunnig necesary to work correctly on RHEL7.

### Requirements

Yum repsitorios with access to docker rpms,

### Dependencies

N/A

### Example Playbook

    - hosts: servers
      roles:
        - { role: docker }

docker ansible role default variables
-------------------------------------

#### Sections

-   docker management
-   docker lvm storage management
-   docker private registry management

### docker management

`yum_common_repos`

> Docker package name (rpm)

    docker_package: docker

`docker_role_debug`

> Debug some output for the role execution (bool)

    docker_role_debug: false

    docker_start: true

    docker_file_max: 120000

### docker lvm storage management

`docker_lvm`

> Configure docker to use lvm as storage (bool)

    docker_lvm: false

`docker_storage_device`

> Disk used as pv for LVM

    docker_storage_device: /dev/sdb

`docker_vg_size`

> Size to use for the vg on the pv

    docker_vg_size: 10GB

### docker private registry management

`docker_login_user`

> User to login on docker registry

    docker_login_user: false

    docker_private_registry: false

    docker_private_registry_insecure: false

Changelog
---------

**docker**

This project adheres to Semantic Versioning and human-readable
changelog.

### docker master - unreleased

##### Added

-   First addition

##### Changed

-   First change

### docker v0.0.1 - 2017/07/12

##### Added

-   Initial version

Copyright
---------

docker

Copyright (C) 2017/07/12 Raúl Melo
&lt;<raul.melo@opensolutions.cloud>&gt;

LICENSE
