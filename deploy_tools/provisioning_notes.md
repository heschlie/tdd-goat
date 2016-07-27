Provisioning a new site
=======================

## Required packages:

* nginx
* Python 3
* Git
* pip
* virtualenv

e.g.,, on Ubuntu:

    sudo apt install nginx git python3 python3-pip
    sudo pip3 install virtualenv

## Nginx Virtual Host config

* See nginx.template.conf
* Replace SITENAME with, e.g., staging.my-domain.com

## Systemd service

* see gunicorn-systemd.template.conf
* Replace SITENAME with, e.g., staging.my-domain.com

## Directory structure

Assume we have the account /home/listuser

/home/listuser
sites/
└── SITENAME
    ├── database
    ├── source
    ├── static
    └── virtualenv
