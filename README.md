# lxc-bootstrap

A basic Ansible playbook to bootstrap newly-created LXC instances by running
a few tasks including the following:

- Setting the time zone
- Updating system packages
- Installing commonly installed packages

## Assumptions

- LXC instance is running Debian
- `remote_user` can SSH to instance through the use of a SSH public key

## Usage

Determine the IP address of the LXC container, update `hosts` giving the
container the desired role(s), and run the playbook with the following:

```
ansible-playbook site.yml
```

### Roles

- development
- python
