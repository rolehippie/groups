# groups

[![Build Status](https://cloud.drone.io/api/badges/rolehippie/groups/status.svg)](https://cloud.drone.io/rolehippie/groups)

Ansible role to configure groups

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
