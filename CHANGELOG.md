# Changelog

All notable changes to this project will be documented in this file.

## [1.2.2] - 2024-11-01

### Features

- Ensure rclone will run on next boot if it misses.
- [**breaking**] Remove podman-compose.
- Enable podman auto-update timer and configure.

### Refactor

- Use universal module to install rclone.

## [1.2.1] - 2024-09-30

### Bug Fixes

- Fix condition when deciding to execute task.
- Syntax update.

### Features

- Specify variable on role.
- Only execute when variable list contains kubernetes.

### Styling

- More specific on task function.

## [1.2.0] - 2024-07-28

### Bug Fixes

- Collection name.
- Variable name and condition.
- Role name dependencies.

### Documentation

- [**breaking**] Remove repository from pyproject file.

### Features

- [**breaking**] Merge podman and kubernetes role into containers role. (#9)
- [**breaking**] Remove poetry configuration, use pdm instead.
- Install dev tools and python tools.
- [**breaking**] Migrate ansible setup into its own role.
- Install ruff.
- Add setuptools to dev role.
- Add argument_spec file for role.
- Add git-cliff tool.
- [**breaking**] Remove password prompt.
- Ignore .pdm-python file.
- Install kubectl.
- [**breaking**] Merge podman and kubernetes role into one.

### Refactor

- [**breaking**] Remove unused variable.

### Miscellaneous Tasks

- Setup pre-commit config file.

### Styling

- Change variable name with role name prefix.

## [1.1.0] - 2024-04-04

### Bug Fixes

- Missing dependencies.

### Features

- Variable to specify cluster type.
- Install helm kubernetes package manager.
- Add `home_config` role to playbook.
- Create directory for storing settings.
- [**breaking**] Setup `group_vars` depending on OS.

### Refactor

- Always to set permit traffic for samba.
- Rename variable and install only if type is `kind`.

### Revert

- Role back to named 'kubernetes'.

## [1.0.0]

### Bug Fixes

- Add GitHub Action. (#5)
- (Ansible-Lint): Change variable name.
- [**breaking**] Remove deprecated playbook, fix tag name.
- Update and install `ansi_colle-mods`.

### Features

- Add GitHub Action. (#5)
- Migrate dependencies into its own file.
- [**breaking**] Remove repeated role.
- [**breaking**] Delete tests directory.
- Use `git-cliff` instead of `antsibull-changelog`. (#6)
- Add `ansible-lint` to pre-commit config file.
- Kubernetes roles for install and setup kubernetes.
- New playbook for testing locally.
- [**breaking**] Remove ansible.cfg file from repo.

### Refactor

- Rename to kind instead of kubernetes.
- Move inventory outside repo.
- Remove depreated file.
<!-- generated by git-cliff -->
