amaabca.newrelic-inode-plugin
=========

[![Build Status](https://travis-ci.org/amaabca/ansible-newrelic-inode-plugin.svg)](https://travis-ci.org/amaabca/ansible-newrelic-inode-plugin)

Installs https://github.com/Foild/newrelic-inode-plugin on Ubuntu

Requirements
------------

    pip install -r requirements.txt

Role Variables
--------------


Dependencies
------------

Server dependencies: 
 - https://www.ruby-lang.org/en/
 - https://rubygems.org/gems/bundler

Development dependencies:
  - https://pypi.python.org/pypi/pip
  
    pip install virtualenv
    virtualenv .
    pip install -r requirements.txt

Example Playbook
----------------

     - { role: ansible-newrelic-inode-plugin, 
           newrelic_inode_plugin_license_key: "{{ secrets.newrelic_license }}", 
           newrelic_inode_plugin_hostname: "{{ hostvars[inventory_hostname]['ansible_default_ipv4']['address'] }}" }

License
-------

MIT

Author Information
------------------

http://github.com/amaabca
