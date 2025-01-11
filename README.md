# Ansible Role: Remi Repository

An Ansible Role that installs the Remi Repository on RedHat/CentOS.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```yaml
remi_repo_url: "http://rpms.remirepo.net/enterprise/remi-release-{{ ansible_distribution_major_version }}.rpm"
remi_repo_gpg_key_url: "https://rpms.remirepo.net/enterprise/{{ ansible_distribution_major_version }}/RPM-GPG-KEY-remi"
```

## Dependencies

None.

## Example Playbook

```yaml
- hosts: servers
  roles:
    - { role: farisc0de.remi }
```

## License

MIT
