osp-servers
=========

Creates openstack instances, looping through vars defined in vars folder.

Requirements
------------
Requires openstack to be connectable from the localhost this module runs on.

Role Variables
--------------
Defined in the vars folder;
cloud_instances:

  - webserver_name: app1
    webserver_group: apps
    deployment: QA
    flavor_name: m2.small
    security_groups: apps

  - webserver_name: app2
    webserver_group: apps
    deployment: QA
    flavor_name: m2.small
    security_groups: apps

  - webserver_name: db
    webserver_group: appdbs
    deployment: QA
    flavor_name: m2.small
    security_groups: db

  - webserver_name: frontend
    webserver_group: frontends
    deployment: QA
    flavor_name: m2.small
    security_groups: frontend

Dependencies
------------


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: osp-servers }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).