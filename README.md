Ansible role for podman
=======================

Install podman and its ecosystem.

Requirements
------------

- **OS Platforms:** RHEL 8/9, Debian, Ubuntu 22.04+

Role Variables
--------------

| Variable Name | Default Value | Description |
| :--- | :--- | :--- |
| `podman_extras_packages` | `podman-docker, buildah, skopeo` | Additional packages for podman ecosystem |


Example Playbook
----------------

```yaml
- name: Deploy podman
  hosts: servers
  become: true
  roles:
    - role: laxathom.podman
```

License
-------

MIT

Author Information
------------------

- **Owner:**  laxahom
