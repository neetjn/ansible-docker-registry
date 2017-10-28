<a target='_blank' rel='nofollow' href='https://app.codesponsor.io/link/ymhxqZ47jLBFuVrU2iywqLGC/neetjn/ansible-docker-registry'>
  <img alt='Sponsor' width='888' height='68' src='https://app.codesponsor.io/embed/ymhxqZ47jLBFuVrU2iywqLGC/neetjn/ansible-docker-registry.svg' />
</a>

# ansible-docker-register

Ansible playbook for setting up and provisioning a private docker registry.

This ansible playbook will install docker if not done so already, and any other necessary packages or modules. This playbook also supports NGINX proxying if a host is specified in the NGINX host group.

### Variables

* *remote_host*: ...
* *ansible_ssh_user*: ...
* *ansible_ssh_pass*: ...
* *registry_port*: ...
* *registry_user*: ...
* *registry_pass*: ...

### Requirements

* ansible 2 - 2.3
    * *due to a change in version 2.4 defined [here](https://github.com/ansible/ansible/issues/31041), any version of ansible above 2.3.x is not recommended*

### Use

Clone the repository
```bash
git clone https://github.com/neetjn/ansible-docker-registry.git

cd ansible-docker-registry

ansible-playbook playbook.yml -i hosts
```

---

Copyright (c) 2017 John Nolette Licensed under the MIT license.