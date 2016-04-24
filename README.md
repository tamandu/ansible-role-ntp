# ansible-role-ntp

This role configures ntp.

## Requirements

None.

## Role Variables

variable    | required | default | choice | comment
----------- | -------- | ------- | ------ | -------------------
ntp_server  | yes      |         |        | list of ntp server

## Dependencies

None.

## Example Playbook

```yml
- hosts: servers
  roles:
    - ntp
```

*Inside `vars/main.yml`*:  
Variables must be defined by list.
```yml
ntp_server:
  - ntp0.sample.local
  - ntp1.sample.local
  - ntp2.sample.local
```

## License

MIT

## Author Information
