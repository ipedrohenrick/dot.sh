# DotFiles

## Install

```sh
ansible-playbook --ask-become-pass -l <nome-do-host> playbook.yml
```

## After install steps

See [after-install.md](docs/after-install.md)

## Troubleshoting

###  Timeout in sudo fingerprint verification

Ansible cannot escalate privileges with fingerprint, so it is necessary to disable this function to run the playbook,
the `utils/change_fingerprint.sh` script is included for this.
