Role Name
=========

This role installs a docker registry cache for use on an openstack cluster using master und slave instances.
It installs the actual register cache on the master instance (grouped as [master]) and configures a pointer on the slaves to this register cache.

Requirements
------------

Ubuntu 16.04

Role Variables
--------------

cache_port defines the mainport for the cache container.
main_dir gives the path on the master instance, on where the cached files are stored.


Example Playbook
----------------

Simply instal this role and add it to your playbook.


	- hosts: all
	  roles:
		- dockerRegCache

License
-------

BSD

Author Information
------------------

For more Information: https://wiki.cebitec.uni-bielefeld.de/bibiserv-1.25.2/index.php/Setup_Registry_Proxy_Cache
