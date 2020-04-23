# Install Oracle Database 18c with Ansible

These roles configure Oracle Database prerequisites and install it for CentOS 7.

## Requirements

- CentOS 7.7 or later
- Ansible 2.9
- Installation media file distributed by oracle.com

## Create VM and install the Oracle Database software

Place the installation media file into roles/oracle19c/files/ and run vagrant as follows;

```
$ cp /foo/bar/LINUX.X64_193000_db_home.zip roles/oracle19c/files/
$ ansible-playbook -i inventory.yml playbook.yml oracle -k -K
```
