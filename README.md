# Simple sudoers role

This role installs the sudo package, ensures that /etc/sudoers.d is included and
creates or removes sudoers files in /etc/sudoers.d.

## Variables

 * sudoers_filename - file name in /etc/sudoers.d (required)
 * sudoers - A list of users who have some sort of sudo access.
   * defaults: []
   * example: Check ```ansible-sudoers.yml``` playbook for examples.
 * sudoers_remove - if enabled, removes /etc/sudoers.d/{{ sudoers\_filename }} instead
   of creating it.
   * default: false
