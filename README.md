# Ansible Role: Installs Java 8 JDK

Java 8 JDK installation on Linux.

Travis status:   [![Build Status](https://travis-ci.org/KAMI911/ansible-role-java-oracle-jdk8.svg?branch=master)](https://travis-ci.org/KAMI911/ansible-role-java-oracle-jdk8)
Code Climate status: [![Code Climate](https://codeclimate.com/github/KAMI911/ansible-role-java-oracle-jdk8/badges/gpa.svg)](https://codeclimate.com/github/KAMI911/ansible-role-java-oracle-jdk8)
Test Coverage status: [![Test Coverage](https://codeclimate.com/github/KAMI911/ansible-role-java-oracle-jdk8/badges/coverage.svg)](https://codeclimate.com/github/KAMI911/ansible-role-java-oracle-jdk8/coverage)

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

    java_update: 141

Java minor version.

    java_build: "01"

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

This role was created in 2016-2017 by Kálmán Szalai - KAMI
