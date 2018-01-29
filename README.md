[![Build Status](https://travis-ci.org/while-true-do/ansible-role-repo-webtatic.svg?branch=master)](https://travis-ci.org/while-true-do/ansible-role-repo-webtatic)

# Ansible Role: Repo-Webtatic
| A role that installes yum repository for updated web related packages (Webtatic).

## Motivation

This role is needed to get access to updated web related packages (Webtatic).

## Installation

Install from [Ansible Galaxy](https://galaxy.ansible.com/while-true-do.repo-webtatic)

```
ansible-galaxy install while-true-do.repo-webtatic
```

Install from [Github](https://github.com/while-true-do/ansible-role-repo-webtatic)

```
git clone https://github.com/while-true-do/ansible-role-repo-webtatic.git while-true-do.repo-webtatic
```

## Requirements

**Used Modules**

-   [package_module](http://docs.ansible.com/ansible/latest/package_module.html)

## Role Variables
```yaml
# defaults/main.yml
# You can change the state (present|absent)
wtd_repo_webtatic_state: present

wtd_repo_webtatic_packages:
  - "https://mirror.webtatic.com/yum/el7/webtatic-release.rpm"
```

## Dependencies

None.

## Example Playbook

Simple Example:

```yaml
- hosts: servers 
  roles:
    - { role: while-true-do.repo-webtatic }
```

## Testing

All tests should be put in [test directory](./tests/).

## Contribute / Bugs

Thank you so much for considering to contribute. Every contribution helps us.
We are really happy, when somebody is joining the hard work. Please have a look 
at the links first.

-   [Contribution Guidelines](./docs/CONTRIBUTING.md)
-   [Create an issue or Request](https://github.com/while-true-do/ansible-role-repo-webtatic/issues)
-   [See who was contributing already](https://github.com/while-true-do/ansible-role-repo-webtatic/graphs/contributors)

## License
This work is licensed under a [BSD License](https://opensource.org/licenses/BSD-3-Clause).

## Author Information

Blog: [blog.while-true-do.org](https://blog.while-true-do.org)

Mail: [hello@while-true-do.org](mailto:hello@while-true-do.org)
