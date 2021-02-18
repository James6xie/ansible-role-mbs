## Ansible Role: mbs
This mbs role is used in the CentOS Infra.

It surely depends (see dependencies below) on some other roles.

See also [ansible-infra-playbooks](https://github.com/CentOS/ansible-infra-playbooks) directory to see how the tree/structure is organized

### Variables
See [defaults variables and explanations](defaults/main.yml)

### Dependencies

This role depends on an existing postgresql instance + fedmsg-hub.

All those roles are declared in our [requirements.yml](https://github.com/CentOS/ansible-infra-playbooks/blob/master/requirements-production.yml) file.

### Development

Molecule tests use vagrant so you need a working vagrant installation in your host machine.

Running molecule tests require the following python libraries:

- molecule
- molecule-vagrant
- python-vagrant

Tests can be executed by running:

```sh
molecule test
```

### License
MIT (see [LICENSE](LICENSE) file)

