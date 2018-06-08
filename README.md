# ansible-role-linuxhq

[![Build Status](https://travis-ci.org/linuxhq/ansible-role-linuxhq.svg?branch=master)](https://travis-ci.org/linuxhq/ansible-role-linuxhq)
[![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-linuxhq-blue.svg?style=flat)](https://galaxy.ansible.com/linuxhq/linuxhq)
[![License](https://img.shields.io/badge/license-GPLv3-brightgreen.svg?style=flat)](COPYING)

Installs a linuxhq package specific RPM repository.

## Requirements

None

## Role Variables

Available variables are listed below, along with their default values

    linuxhq_enabled: false
    linuxhq_gpgcheck: false
    linuxhq_repo_gpgcheck: true
    linuxhq_sslcacert: /etc/pki/tls/certs/ca-bundle.crt
    linuxhq_sslverify: true
    linuxhq_source_enabled: false
    linuxhq_source_gpgcheck: false
    linuxhq_source_repo_gpgcheck: true
    linuxhq_source_sslcacert: /etc/pki/tls/certs/ca-bundle.crt
    linuxhq_source_sslverify: true

## Dependencies

None

## Example Playbook

    - hosts: servers
      roles:
        - role: linuxhq.linuxhq
          linuxhq_pkg: snoopy

## Partners

[![packagecloud](http://dka575ofm4ao0.cloudfront.net/pages-transactional_logos/retina/10543/gKme3F4XRaC5EyKJzKsA)](https://packagecloud.io)

Do you need trustworthy hosted package repositories?  Then packagecloud is for you.

A big thank you to packagecloud for supporting the open source community!

## License

Copyright (C) 2018 Taylor Kimball <tkimball@linuxhq.org>

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <http://www.gnu.org/licenses/>.
