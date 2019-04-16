config-tower
=========

Role to configure ansible tower job templates and workflow

Requirements
------------
vars/main.yml | Very important file to review. All the variable values are set there. Please do not make any changes in the file

Role Variables
--------------
        - TOWER_GUID: <Ansible Tower Homework GUID from mail>
        - OSP_GUID: <Openstack for Ansible GUID from mail>
        - OPENTLC_LOGIN: <username-company.com>
        - OPENTLC_PASSWORD: <your openlc account password>
        - GITHUB_REPO: https://github.com/<githubhandler>/ansible_advance_homework
        - JQ_REPO_BASE: http://www.opentlc.com/download/ansible_bootcamp
        - REGION: <enter region name example us-east-1>
        - RH_MAIL_ID: <your mail id for dynamic inventory tag>


Dependencies
------------


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: localhost
      roles:
         - { role: config-tower }
	  vars:
        - TOWER_GUID: <Ansible Tower Homework GUID from mail>
        - OSP_GUID: <Openstack for Ansible GUID from mail>
        - OPENTLC_LOGIN: <username-company.com>
        - OPENTLC_PASSWORD: <your openlc account password>
        - GITHUB_REPO: https://github.com/<githubhandler>/ansible_advance_homework
        - JQ_REPO_BASE: http://www.opentlc.com/download/ansible_bootcamp
        - REGION: <enter region name example us-east-1>
        - RH_MAIL_ID: <your mail id for dynamic inventory tag>

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).