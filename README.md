[![Ansible Role](https://img.shields.io/ansible/role/18529.svg)](https://galaxy.ansible.com/xtrinch/kiosk/)

Ansible role: kiosk
=========

Creates a chromium website kiosk out of ubuntu server with a very light stack of X and openbox. Essentially, it creates two separate systemd services: one for running x environment (startx), and one for running chromium. Chromium is restarted upon exiting.

Requirements
------------

- a clean installation of ubuntu server

Installation
------------

Role can be installed via ansible-galaxy or via cloning this repository into roles/.
For more info, see: https://galaxy.ansible.com/xtrinch/kiosk/

Role Variables
--------------

    website_url: "http://www.google.com"
    kiosk_user: test

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: xtrinch.kiosk, kiosk_user: test, website_url: "http://www.google.com" }

License
-------

MIT
