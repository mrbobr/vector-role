Role Name
=========

[Vector](https://vector.dev/) deploy on EL7 

Requirements
------------

EL7 OS

Role Variables
--------------
Version & download url for vector package (list of versions on https://vector.dev/download/)
```yaml
vector_version: "0.22.2"
vector_url: "https://packages.timber.io/vector/{{ vector_version }}/vector-{{ vector_version }}-1.x86_64.rpm"
```

Example Playbook
----------------

    - name: Install Vector
      hosts: vector servers
      roles:
        - vector-role

License
-------

MIT
