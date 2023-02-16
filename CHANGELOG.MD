# CHANGELOG

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
