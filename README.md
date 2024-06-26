# zeevo.zookeeper

Deploy Zookeeper for use with clustered applications.

## Requirements

This role depends on `docker` being available on hosts.

## Role Variables

```yml
zookeeper_home_dir: /data/zookeeper # Directory where zookeeper will store its data
zookeeper_user: admin # Zookeeper user
zookeeper_group: zookeeper # Zookeeper group
```

## Example Playbook

Use `zeevo.zookeeper` in a Playbook.

```yml
# Playbook `zookeeper.yml`

- name: zookeeper
  hosts: zookeeper
  become: true
  roles:
    - zeevo.zookeeper
```

## License

MIT

## Author Information

This role was created by and is maintained by [Zeevo](https://zeevo.io).
