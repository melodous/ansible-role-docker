Role Name
=========

This role install docker engine on the server, and configure the logging, monitoring and tunnig necesary to work correctly on RHEL7.

Requirements
------------

Yum repsitorios with access to docker and pip rpms

Dependencies
------------

N/A

Example Playbook
----------------

.. code::

  - hosts: servers
    roles:
      - { role: docker }
