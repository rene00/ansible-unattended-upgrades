# ansible-role: unattended-upgrades

**This repo is a Work In Progress**

## Description
An ansible role to install and configure automatic installation of security upgrades for Debian based distributions.

## Role Variables
All variables which can be overridden are stored in [defaults/main.yml](defaults/main.yml) file as well as in table below.

| Name                                                 | Default Value | Description                                                                                                                 |
| --------------                                       | ------------- | -----------------------------------                                                                                         |
| `unattended_upgrades_mail`                           |               | Send email to this address for problems or packages upgrades                                                                |
| `unattended_upgrades_mailreport`                     |               | Set this value to one of: "always", "only-on-error" or "on-change"                                                          |
| `unattended_upgrades_remove_unused_kernel_packages`  |               | Remove unused automatically installed kernel-related packages                                                               |
| `unattended_upgrades_minimalsteps`                   |               | Split the upgrade into the smallest possible chunks so that they can be interrupted with SIGTERM                            |
| `unattended_upgrades_remove_new_unused_dependencies` |               | Do automatic removal of newly unused dependencies after the upgrade                                                         |
| `unattended_upgrades_remove_unused_dependencies`     |               | Do automatic removal of unused packages after the upgrade                                                                   |
| `unattended_upgrades_install_on_shutdown`            |               | Install all updates when the machine is shutting down instead of doing it in the background while the machine is running    |
| `unattended_upgrades_automatic_reboot`               |               | Automatically reboot *WITHOUT CONFIRMATION* if the file `/var/run/reboot-required` is found after the upgrade               |
| `unattended_upgrades_automatic_reboot_withusers`     |               | Automatically reboot even if there are users currently logged in when `Unattended-Upgrade::Automatic-Reboot` is set to true |
| `unattended_upgrades_automatic_reboot_time`          |               | If automatic reboot is enabled and needed, reboot at the specific time instead of immediately                               |
