# CHANGELOG

## Unreleased

### Breaking

- Drop support for Ansible 2.9, migrate module names to FQCNs.

### Fixed

- Squished annoying bug that prevented redownloading binary on version, arch or OS change ([fb4c0bf](https://github.com/kazauwa/ansible-role-headscale/commit/fb4c0bf51d32e3c4ae24f79810a76d4260c3c1e1)).

## 1.4.0 (2024-03-18)

### Fixed

- Fixed faulty logic causing the role to fail on the initial run ([#5](https://github.com/kazauwa/ansible-role-headscale/pull/6)).

### Changes

- Parametrize target OS in headscale download link ([255be2b](https://github.com/kazauwa/ansible-role-headscale/commit/255be2b74954418e7085fa9e24d1a5e05d10e69c)).

## 1.3.1 (2023-08-09)

### Changes

- Add support for config template, see `headscale_config_template` variable ([80c6157](https://github.com/kazauwa/ansible-role-headscale/commit/80c6157e31d98a6534c226230ea4ad2ca8e27950))
- Bump default Headscale version to v0.22.3 ([96f42b3](https://github.com/kazauwa/ansible-role-headscale/commit/96f42b337db89e78919b4b9adb9382887c4f4c73))


## 1.3.0 (2023-02-16)

### Breaking

- Rename `namespaces` to `users` to align with changes to Headscale (see [0.19.0 release notes](https://github.com/juanfont/headscale/blob/main/CHANGELOG.md#0190-2023-01-29)) ([d1a83ac](https://github.com/kazauwa/ansible-role-headscale/commit/d1a83ac74239f32756c8ae4aa0224c4ac01cf930))

### Changes

- Fix triggering changed state in Ansible caused by `headscale_pid_dir` mode ([be60f3c](https://github.com/kazauwa/ansible-role-headscale/commit/be60f3cf31578e68a27e6a86727ad6709c319948))
- Restart Headscale after update ([3cc93d7](https://github.com/kazauwa/ansible-role-headscale/commit/3cc93d74267212c33dc2f7858247c399db030173))


## 1.2.0 (2022-12-06)

### Changes

- Bump Headscale version to the latest ([8fbfa51](https://github.com/kazauwa/ansible-role-headscale/commit/8fbfa516acd54e6cd325973d7c55d7d0243f7ab5))
- Reload Headscale on config change instead of restarting ([fafae46](https://github.com/kazauwa/ansible-role-headscale/commit/fafae466f9584ce6c0e9fdeb638917507630303a))
- Update docs for `headscale_enable_routes` and `headscale_exit_nodes` variables ([ac67ff0](https://github.com/kazauwa/ansible-role-headscale/commit/ac67ff0d07954ea7ec8890e587bb97216ba4464d))

## 1.1.0 (2022-05-29)

### Changes

- Add support for enabling routes and exit nodes ([b74e0e7](https://github.com/kazauwa/ansible-role-headscale/commit/b74e0e7f822aa9da90d272a7e3016f8fd39eafee))
