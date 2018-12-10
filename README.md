CenterDevice artifacts installation
=========

This role can be used to install CenterDevice artifacts from a AWS S3 bucket

[![Build Status](https://travis-ci.org/Rheinwerk/ansible-role-install_cd_build_artifacts.svg?branch=master)]((https://travis-ci.org/Rheinwerk/ansible-role-install_cd_build_artifacts)

Requirements
------------

None.

Role Variables
--------------

There is one main variable that drives this role: `_cd_build`. It is a map that contains all configuration and settings for this role.
Please see `defaults/main.yml` for details.

Dependencies
------------

None.


Example Playbook
----------------

The general contract of this role is to take the variables map `_cd_build` from `defaults/main.yml` as a template for your configuration and pass that configuration as a parameter to this role.

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      var:
        CD_BUILD_ARTIFACTS:
          ...
      roles:
        - { role: install_cd_build_artifacts, _cd_build: "{{ CD_BUILD_ARTIFACTS }}", tags: ['cd-build-artifacts'] }

License
-------

Please see LICENSE.

Author Information
------------------

Original author is [Alexander Berresch](https://github.com/aberresch) as member of the [Rheinwerk](https://github.com/Rheinwerk) project.


