Ansible role: kiosk
=========

Creates a chromium website kiosk out of ubuntu server with a very light stack of X and openbox.

Requirements
------------

- a clean installation of ubuntu server

Role Variables
--------------

    website_url: "http://www.google.com"
    kiosk_user: test

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: trina.kiosk, kiosk_user: test, website_url: "http://www.google.com" }

License
-------

MIT
