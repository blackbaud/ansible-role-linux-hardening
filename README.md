linux-hardening
===============
[![status](https://travis-ci.org/blackbaud/ansible-role-linux-hardening.svg?branch=master)](https://travis-ci.org/blackbaud/ansible-role-linux-hardening)

This role hardens linux hosts (Centos, Ubuntu, and Amazon Linux).  It follows the CIS standards, although it doesn't do everything that is recommended.

Requirements
------------

None

Role Variables
--------------

There are a number of variables defined in the defaults and vars directories, but none of them should need to be updated in order to run properly.

Dependencies
------------

There are no dependencies for this role.  

Installation Instructions
-------------------------

To install this role in your local ansible directory, create a file called requirements.yml in the base directory with the following:

    # from GitHub
    - src: https://github.com/blackbaud/ansible-linux-hardening

 Then run the ansible-galaxy command to add the role:
 
    $ ansible-galaxy install -r requirements.yml

Example Playbook
----------------

Include the role in your playbook to harden your linux servers:

    - hosts: servers
      roles:
         - ansible-role-linux-hardening

License
-------

MIT

Author Information
------------------

Blackbaud
Created in 2016 by [Blackbaud](http://blackbaud.com/)