# varnish

[![Build Status](https://travis-ci.com/iroquoisorg/ansible-role-varnish.svg?branch=master)](https://travis-ci.com/iroquoisorg/ansible-role-memcached)

Ansible role for varnish

This role was prepared and tested for Ubuntu 16.04.

# Installation

`$ ansible-galaxy install iroquoisorg.varnish`

# Default settings

```

varnish_package_name: "varnish"
varnish_version: "4.1"

varnish_use_default_vcl: true
varnish_default_vcl_template_path: default.vcl.j2

varnish_default_backend_host: "127.0.0.1"
varnish_default_backend_port: "8080"

varnish_error_template: error.html.j2

varnish_listen_port: "80"
varnish_secret: "cad79ccc-6b39-4780-996a-6f93aa53331b"
varnish_config_path: /etc/varnish
varnish_limit_nofile: 131072

varnish_admin_listen_host: "127.0.0.1"
varnish_admin_listen_port: "6082"

varnish_storage: "file,/var/lib/varnish/varnish_storage.bin,256M"
varnish_pidfile: /run/varnishd.pid

```
