sudoersd
=========

This role installs the sudo RPM, ensures that /etc/sudoers.d is included and creates or removes sudoers files in /etc/sudoers.d.

Requirements
------------

None.

Role Variables
--------------

 * sudoers_filename - file name in /etc/sudoers.d (required)
 * sudoers - A list of user who have some sort of sudo access (see example below).
   * default: []
 * sudoers_remove - if enabled, removes /etc/sudoers.d/{{ sudoers\_filename }} instead of creating it.
   * default: false

Dependencies
------------

None.

Example Playbook
----------------


License
-------

BSD

Author Information
------------------

https://github.com/mchlumsky
