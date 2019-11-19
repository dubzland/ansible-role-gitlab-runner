# Ansible Role: GitLab Runner
[![Gitlab pipeline status (self-hosted)](https://git.dubzland.net/dubzland/ansible-role-gitlab-runner/badges/master/pipeline.svg)](https://git.dubzland.net/dubzland/ansible-role-gitlab-runner)

Installs and configures a Runner for GitLab.

## Requirements

Ansible 2.8 or higher.
`python-gitlab` >= `1.5.0` for interacting with the GitLab API.

## Role Variables

Available variables are listed below, along with their default values (see
    `defaults/main.yml` for more info):


## Dependencies

None.

## Example Playbook

```yaml
- hosts: servers
  roles:
    - role: dubzland.gitlab_runner
```

## Post install

Until the `gitlab_runner` Ansible module correctly supports shared runners, the
actual registration will need to be handled manually.

## License

MIT

## Author

* [Josh Williams](https://codingprime.com)
