# Ansible Role: bitcoin-core

[![CI](https://github.com/unxnn/ansible-role-bitcoin-core/workflows/CI/badge.svg?event=push)](https://github.com/unxnn/ansible-role-bitcoin-core/actions?query=workflow%3ACI)

Installs [Bitcoin Core](https://bitcoincore.org/) on RedHat/CentOS and Debian/Ubuntu servers.

## Role configuration

Full description of the role parameters can be found in the [**defaults/main.yml**](defaults/main.yml) file.

Example:

```yaml
---

- hosts: localhost
  become: true
  roles:
    - unxnn.bitcoin_core
  vars:
    bitcoin_version: 0.20.1
    bitcoin_user: non-default
    bitcoin_group: custom-group
    bitcoind_conf_server: 1
    bitcoind_conf_listen: 1
    bitcoind_conf_testnet: 1
    bitcoind_conf_rpcbind_test: 120.120.120.120
    bitcoind_conf_rpcport_test: 8332
```

# Dependenices

None.

# License

MIT
