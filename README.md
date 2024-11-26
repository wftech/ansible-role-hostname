# hostname role

This role sets the hostname of the host to the value specified in the `hostname`
variable.

## Variables


| Variable          | Description                                          |
|-------------------|------------------------------------------------------|
| `hostname_value`  | The hostname to set, default is `inventory_hostname` |
| `hostname_update` | Whether to update the hostname. Default is `true`.   |

# Usage

```yaml

- name: Common setup
  hosts: all

  vars:
      hostname_value: "{{ inventory_hostname }}"
      hostname_update: true
    
  roles:
    - role: wftech.hostname
```

## License

CC0
