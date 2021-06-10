# groups

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&logoColor=white)](https://github.com/rolehippie/groups) [![Testing Build](https://github.com/rolehippie/groups/workflows/testing/badge.svg)](https://github.com/rolehippie/groups/actions?query=workflow%3Atesting) [![Readme Build](https://github.com/rolehippie/groups/workflows/readme/badge.svg)](https://github.com/rolehippie/groups/actions?query=workflow%3Areadme) [![Galaxy Build](https://github.com/rolehippie/groups/workflows/galaxy/badge.svg)](https://github.com/rolehippie/groups/actions?query=workflow%3Agalaxy) [![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/groups)](https://github.com/rolehippie/groups/blob/master/LICENSE) 

Ansible role to create and modify system groups. 

## Sponsor 

[![Proact Deutschland GmbH](https://proact.eu/wp-content/uploads/2020/03/proact-logo.png)](https://proact.eu) 

Building and improving this Ansible role have been sponsored by my employer **Proact Deutschland GmbH**.

## Table of content

* [Default Variables](#default-variables)
  * [groups_extra](#groups_extra)
  * [groups_general](#groups_general)
* [Dependencies](#dependencies)
* [License](#license)
* [Author](#author)

---

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
    system: True
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
    system: True
  - name: group-to-delete
    state: absent
```

## Dependencies

* None

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)
