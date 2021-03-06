.. vim: foldmarker=[[[,]]]:foldmethod=marker

docker ansible role default variables
=====================================

.. contents:: Sections
   :local:

docker management
-----------------

.. envvar:: yum_common_repos

   Docker package name (rpm)

::

  docker_package: docker




.. envvar:: docker_role_debug

   Debug some output for the role execution (bool)

::

  docker_role_debug: false




.. envvar: docker_start

   Start docker on system boot (bool)

::

  docker_start: true




.. envvar: docker_file_max

   Configure number of max files on the kernel

::

  docker_file_max: 120000




docker lvm storage management
-----------------------------

.. envvar:: docker_lvm

   Configure docker to use lvm as storage (bool)

::

  docker_lvm: false




.. envvar:: docker_storage_device

   Disk used as pv for LVM

::

  docker_storage_device: /dev/sdb




.. envvar:: docker_vg_size

   Size to use for the vg on the pv

::

  docker_vg_size: 10GB




docker private registry management
----------------------------------

.. envvar:: docker_login_user

   User to login on docker registry

::

  docker_login_user: false




.. envvar: docker_login_password

   Password to login on docker registry
   ::

     docker_login_password: false




.. envvar: docker_private_registry

   Docker registry address

::

  docker_private_registry: false




.. envvar: docker_private_registry_insecure

   Configure the docker resgustry as insecure (no ca on the server)

::

  docker_private_registry_insecure: false




docker monitoring configuration
-------------------------------

.. envvar:: docker_monitoring

   Enable monitoring of docker container for zabbix

::

  docker_monitoring: true



