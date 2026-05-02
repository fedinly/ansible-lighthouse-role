Role Name
=========
LightHouse is a lightweight GUI interface for ClickHouse.

Requirements
------------

Ansible >= 2.10 (It might work on previous versions, but we cannot guarantee it)

Role Variables
--------------
All variables which can be overridden are stored in defaults/main.yml file as well as in table below.

| Name | Default Value |	Description |
|------|---------------|--------------|
| `lighthouse_access_log_name` | access | Log name that using in nginx conf |
| `lighthouse_dir` | /home/centos/lighthouse | Lighthouse location dir |
| `lighthouse_vcs` | [clickhouse](https://github.com/VKCOM/lighthouse.git) | Link where initial distrib located |
| `nginx_user_name` | centos | Username that using in nginx conf |

Dependencies
------------

List of dependencies:
- Vector role
- Clickhouse role

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - lighthouse

License
-------

MIT

Author Information
------------------

Leonid Fedin
