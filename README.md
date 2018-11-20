[![Build Status](https://travis-ci.org/pescobar/ansible-role-java-oracle.svg?branch=master)](https://travis-ci.org/pescobar/ansible-role-java-oracle)

ansible-role-java-oracle
=========

Install the Java JDK tarball from Oracle to /opt/java

This role will also copy a file to `/etc/profile.d/java.sh` to define `$JAVA_HOME` and `$PATH`

Role Variables
--------------

```
url: "http://download.oracle.com/otn-pub/java/jdk/8u191-b12/2787e4a523244c269598db4e85c51e0c/jdk-8u191-linux-x64.tar.gz"
java_install_folder: "/opt"
```

For this role to work you must define a proper download url and headers.

You can see an example [here](https://tecadmin.net/install-java-8-on-centos-rhel-and-fedora/)

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: ansible-role-java-oracle }

License
-------

GPLv3

Author Information
------------------

Pablo Escobar
