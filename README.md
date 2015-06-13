correcthorse.beanstalkd
=========

An ansible role for installing beanstalkd.

Requirements
------------

This package is not currently available in EPEL 7. This role currently installs a package from the correcthorse RPM repo at packagecloud.io - this RPM is just a rebuild from rawhide.

Role Variables
--------------

| Variable                              | Default				| Notes				|
| :---                                  | :---                                  | :--- 				|
| beanstalkd_address			| 0.0.0.0				| 				|
| beanstalkd_port			| 11300					|				|
| beanstalkd_open_port			| false					|				|
| beanstalkd_user			| beanstalkd				|				|

Dependencies
------------

    - correcthorse.common

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: correcthorse.beanstalkd }

License
-------

MIT

Author Information
------------------

* [Joshua Rusch](https://correct.horse/)
