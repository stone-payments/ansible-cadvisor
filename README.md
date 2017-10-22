stone-payments.cadvisor
============
Role for Ansible which manages cAdvisor.

## Using
You should have Docker already installed and running in the target system in order for this role to work properly. We
suggest using  our [stone-payments.docker](https://github.com/stone-payments/ansible-docker) role for it.

After, you may use a simple playbook like this:
```yaml
- name: install cAdvisor
  hosts: all
  become: true
  include_roles:
    - name: stone-payments.cadvisor
```

## Advanced usage
Trough exposed vars defined in `defaults/main.yml` you may change the cAdvisor docker image (eg. to specify another
version or a different source registry) and the port which cAdvisor will listen on.

## Contributing
Just open a PR. We love PRs!

## License
This role is distributed under the MIT license.
