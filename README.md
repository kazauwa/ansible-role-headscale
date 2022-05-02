# Ansible Role for Headscale

An Ansible Role that installs and manages [Headscale](https://github.com/juanfont/headscale) on Linux.

## Requirements

- Ansible >= 2.9

## Role Variables

- `headscale_version`
  - Default: `0.15.0`
  - Description: version of Headscale to install. List of avaliable versions can be found on [official releases page](https://github.com/juanfont/headscale/releases). Defaults to the latest avaliable.
- `headscale_arch`
  - Default: `amd64`
  - Description: headscale binary target architecture.
- `headscale_user_name`
  - Default: `headscale`
  - Description: name for service user for running Headscale binary.
- `headscale_user_group`
  - Default: `headscale`
  - Description: group for service user for running Headscale binary.
- `headscale_user_uid`
  - Default: `800`
  - Description: uid for service user for running Headscale binary.
- `headscale_user_gid`
  - Default: `800`
  - Description: gid for service user for running Headscale binary.
- `headscale_binary_path`
  - Default: `/usr/local/bin/headscale`
  - Description: path for installing headscale binary.
- `headscale_config_dir`
  - Default: `/etc/headscale`
  - Description: path to headscale configs.
- `headscale_var_data_dir`
  - Default: `/var/lib/headscale`
  - Description: path to headscale data.
- `headscale_pid_dir`
  - Default: `/var/run/headscale`
  - Description: path to headscale socket.
- `headscale_config`
  - Default: `{}`
  - Description: yaml formatted headscale config, consider using [default config](https://github.com/juanfont/headscale/blob/main/config-example.yaml) as a starting point.
- `headscale_acl`
  - Default: `{}`
  - Description: yaml formatted ACL policies. **Make sure** that you've read the [docs](https://github.com/juanfont/headscale/tree/main/docs#policy-acls) on how to use this feature.
- `headscale_namespaces`
  - Default: `[]`
  - Description: list of namespaces to create, e.g. to use with tagOwners.

## Dependencies

None.

## Example Playbook

    - hosts: all
      roles:
        - kazauwa.headscale
      vars:
        headscale_version: '0.15.0'

## License

MIT
