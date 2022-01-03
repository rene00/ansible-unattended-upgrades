# ansible-role: unattended-upgrades

*This repo is a Work In Progress*

## Description
An ansible role to install and configure automatic installation of security upgrades for Debian based distributions.

## Role Variables
All variables which can be overridden are stored in [defaults/main.yml](defaults/main.yml) file as well as in table below.

| Name                             | Default Value | Description                                                        |
| --------------                   | ------------- | -----------------------------------                                |
| `unattended_upgrades_mail`       |               | Send email to this address for problems or packages upgrades       |
| `unattended_upgrades_mailreport` |               | Set this value to one of: "always", "only-on-error" or "on-change" |
