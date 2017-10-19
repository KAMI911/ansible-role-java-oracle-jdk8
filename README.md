# Ansible Role: Installs Java 8 JDK or Server JRE

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

    java_installer_force_overwrite: False

Force to overwrite Java installer.

    java_installer_keep: False

Do not delete Java installer.

    java_installer_local: False

Install local (form Ansible host) JDK/Server JRE instead of downloading on target machine.

    java_type: jdk

Type of Java installer - JDK is: jdk, and Server JRE is: server-jre

    java_version: 8

Java major version.

    java_update: 152

Java minor version.

    java_build: "16"

Java micro version.

    java_platform: linux-x64

Java platform to install.

    java_bins: [ 'javah', 'javap', 'jmap', 'extcheck', 'pack200', 'jrunscript', 'jinfo', 'jcontrol', 'jmc', 'keytool', 'schemagen', 'jjs', 'jvisualvm', 'policytool', 'rmid', 'wsgen', 'javaws', 'javadoc

Update alternatives on these binaries.

    java_bins_priority: 9

Alternatives priority on these binaries.

    java_usr_folder: /usr/java

Location of installed Java home.

    java_latest_folder: /usr/java/latest

Where to link the latest folder.

    java_download_base_url: http://download.oracle.com/otn-pub/java/jdk

Download link of Java installers.

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
