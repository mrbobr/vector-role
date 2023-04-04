Role Name
=========

[Vector](https://vector.dev/) deploy on EL7,8 & ubuntu

Requirements
------------

EL7, EL8, ubuntu OS

Role Variables
--------------
Version & download url for vector package (list of versions on https://vector.dev/download/)
```yaml
vector_version: "0.22.2"
vector_deb_repo_url: 'https://repositories.timber.io/public/vector/cfg/setup/bash.deb.sh'
vector_rpm_repo_url: 'https://repositories.timber.io/public/vector/cfg/setup/bash.rpm.sh'
vector_rpm_url: "https://packages.timber.io/vector/{{ vector_version }}/vector-{{ vector_version }}-1.x86_64.rpm"
vector_rpm_package: "vector-{{ vector_version }}-1.x86_64.rpm"
vector_deb_package: "vector={{ vector_version }}-1"
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
