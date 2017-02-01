Apigee OPDK Cassandra Change Replication Factor
===============================================

This role makes changes to the replication factor 
of a Cassandra keyspace

Requirements
------------

It is assumed that this will be executed on a node running
Cassandra as part of an Edge instance. 

Role Variables
--------------

**keyspace:** Name of the keyspace to update

**opdk_region:** Name of the opdk region to update

**replication_factor:** The replication factor integer to set.
 

Dependencies
------------

- apigee-opdk-setup-default-settings


Example Playbook
----------------

    - hosts: '{{ hosts }}'
      roles:
         - { role: apigee-opdk-setup-default-settings }

License
-------

Apache License Version 2.0, January 2004

Author Information
------------------

Carlos Frias