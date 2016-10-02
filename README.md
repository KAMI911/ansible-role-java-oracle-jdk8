# Ansible Role: Installs Java 8 JDK

Java 8 JDK installation on Linux.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    force_java_install: False

Force to install Java on already installed system.

    keep_java_installer: False

Do not delete Java installer.

    java_version: 8

Java major version.

    java_update: 112

Java minor version.

    java_build: 15

Java micro version.

    java_platform: linux-x64

Java platform to install.

## Dependencies

None.

## Example Playbook

    - hosts: all
      roles:
        - java-oracle-jdk8

## License

MIT / BSD

## Author Information

This role was created in 2016 by Kálmán Szalai
