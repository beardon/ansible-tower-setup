Ansible Tower Deployment
========================

This collection of files provides a complete set of playbooks for deploying
the Ansible Tower software to a single-server installation.

Please read http://releases.ansible.com/ansible-tower/docs/tower_user_guide-latest.pdf for
full documentation and installation/upgrade instructions.

Be sure to edit group_vars/all prior to installation to change your choice
of database password.

To upgrade, set group_vars/all to the existing values prior to running
the setup script again.  Be sure you have the latest setup tarball
prior to attempting an upgrade (e.g, don't try to upgrade to  Tower 1.4.8
using the setup tarball you downloaded when running Tower 1.4.5).

> *WARNING*: The playbook will overwrite the content
> of `pg_hba.conf` and strip all comments from `supervisord.conf`.  Run this
> only on a clean virtual machine if you are not ok with this behavior.
