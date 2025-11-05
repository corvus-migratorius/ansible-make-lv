ansible-make-lv
=========

Role for creating simple lv disks with 1 group and 1 volume

Requirements
------------

None

Role Variables
--------------

None

Dependencies
------------

None

Example Playbook
----------------

```yaml
roles:
    - role: genlab.template
      virtual_group: "group"
      logical_volume: "volume"
      lvm_dev: "/dev/sda"
      size: 100%FREE
      fs_type: ext4
      storage_mountpoint: "/mnt"
      storage_mountpoint_mode: "0700"
      mountpoint_owner: root
      mountpoint_group: root
```

License
-------

BSD

Author Information
------------------

malyuk.ss@genlab.llc
