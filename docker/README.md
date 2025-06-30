Docker Role
===========

This role installs Docker on Debian, Ubuntu and RHEL based systems using the official Docker repositories. It follows best practices from the Docker documentation.

Requirements
------------

Ansible 2.12 or higher.

Role Variables
--------------

```yaml
docker_compose_plugin: true   # install docker-compose plugin
docker_user: docker           # user created to run docker
docker_uid: 997               # uid for docker user
docker_group: docker          # group for docker
docker_gid: 997               # gid for docker group
```

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: all
  become: true
  roles:
    - role: docker
```

License
-------

MIT
