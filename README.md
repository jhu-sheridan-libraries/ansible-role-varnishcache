Varnish Cache Ansible Role
=========

Ansible role to install and configure Varnish Cache (5.x by default)

Requirements
------------
The only assumed requirement is that CentOS or RedHat 7 is on the target host.

Role Variables
--------------
* varnish_backend_default_host: (optional)
  - This will set the host of the "backend default" configuration in default.vcl
* varnish_backend_default_port: (optional)
  - This will set the port of the "backend default" configuraiton in default.vcl
* varnish_version: (optional)
  - This sets the major version that will be installed.  Currently only tested with 5.

Dependencies
------------

No other roles or variables are required.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      roles:
         - { role: ansible-role-varnishcache, varnish_backend_default_host: 127.0.0.1, varnish_backend_default_port: 6081, varnish_version: 5 }

License
-------

TBD

Author Information
------------------
Johns Hopkins Sheridan Libraries
  - Derek Belrose <dbelrose@jhu.edu>
