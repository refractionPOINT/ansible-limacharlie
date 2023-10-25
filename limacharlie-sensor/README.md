limacharlie-sensor
=========

This role downloads and installs the LimaCharlie EDR sensor.

Requirements
------------

This role uses `get_url` to download sensor binaries and debs from LimaCharlie.

Role Variables
--------------

* vars/main.yml
  * `installation_key` must be set
* playbook vars or --extra-vars
  * `deployment`
    * `deb`
    * `binary`

Example Playbook
----------------

Example playbook is in `limacharlie-sensor.yml`

### Usage:

#### Deploy via binary 
```
ansible-playbook limacharlie-sensor.yml --extra-vars "deployment=binary"
```
#### Deploy via deb file
```
ansible-playbook limacharlie-sensor.yml --extra-vars "deployment=deb"
```
