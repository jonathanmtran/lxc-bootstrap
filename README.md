# lxc-bootstrap

A basic Ansible playbook to bootstrap newly-created LXC instances by running
a few tasks including the following:

- Setting the time zone
- Updating system packages
- Installing commonly installed packages

## Usage

Determine the IP address of the LXC container and run the playbook with the
following:

```
ansible-playbook -i <ip_address>, site.yml
```

Note the comma after the IP address.
Credit: https://coderwall.com/p/tx91cw/run-ansible-on-a-single-host
