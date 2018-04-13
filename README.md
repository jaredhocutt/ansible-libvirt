# Libvirt

Installs and configures libvirt.

## Requirements

None

## Role Variables

| Variable              | Required | Default | Description                                              |
| --------------------- | -------- | ------- | -------------------------------------------------------- |
| `libvirt_allow_group` | :x:      | `wheel` | The group to allow access to libvirt via a polkit polcy. |

## Dependencies

None

## Example Playbook

```yaml
- hosts: localhost
  vars:
    libvirt_allow_group: wheel
  roles:
      - jaredhocutt.libvirt_allow_group
```
