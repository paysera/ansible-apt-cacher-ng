# Ansible Role: apt-cacher-ng

[![Build Status](https://travis-ci.com/paysera/ansible-apt-cacher-ng.svg?branch=master)](https://travis-ci.com/stankoviciuslukas/ansible-apt-cacher-ng)

An Ansible Role to install and configure apt-cacher-ng on Debian/Ubuntu

## Requirements

None.

## Role Variables

Define this in your playbook to set up on client. This will setup Proxy on machine.

    apt_cacher_ng_server: "1.1.1.1"

Default values used for apt-cacher-ng config. You can specify which port and CacheDir to use for apt-cacher-ng.

    apt_cacher_ng_port: 3142
    apt_cacher_ng_cache_dir: /var/cache/apt-cacher-ng

## Dependencies

None.

## Example Playbook

    - hosts: all
      roles:
        - ansible-apt-cacher-ng

## License

MIT / BSD
