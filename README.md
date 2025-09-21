# groups

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&logoColor=white)](https://github.com/rolehippie/groups)
[![General Workflow](https://github.com/rolehippie/groups/actions/workflows/general.yml/badge.svg)](https://github.com/rolehippie/groups/actions/workflows/general.yml)
[![Readme Workflow](https://github.com/rolehippie/groups/actions/workflows/docs.yml/badge.svg)](https://github.com/rolehippie/groups/actions/workflows/docs.yml)
[![Galaxy Workflow](https://github.com/rolehippie/groups/actions/workflows/galaxy.yml/badge.svg)](https://github.com/rolehippie/groups/actions/workflows/galaxy.yml)
[![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/groups)](https://github.com/rolehippie/groups/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/role-rolehippie.groups-blue)](https://galaxy.ansible.com/rolehippie/groups)

Ansible role to create and modify system groups.

## Sponsor

Building and improving this Ansible role have been sponsored by my current and previous employers like **[Cloudpunks GmbH](https://cloudpunks.de)** and **[Proact Deutschland GmbH](https://www.proact.eu)**.

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [groups_extra](#groups_extra)
  - [groups_general](#groups_general)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.10`

## Default Variables

### groups_extra

List of extra groups

#### Default value

```YAML
groups_extra: []
```

#### Example usage

```YAML
groups_extra:
  - name: sftp
    system: true
  - name: group-to-delete
    state: absent
```

### groups_general

List of global groups

#### Default value

```YAML
groups_general: []
```

#### Example usage

```YAML
groups_general:
  - name: sftp
    system: true
  - name: group-to-delete
    state: absent
```

## Discovered Tags

**_groups_**

## Dependencies

- None

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)
