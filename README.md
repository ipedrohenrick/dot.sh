# DotFiles

## Install

```sh
ansible-playbook --ask-become-pass -l <nome-do-host>
```

## After install steps

See [after-install.md](docs/after-install.md)

## Troubleshoting

###  Timeout in sudo fingerprint verification

Ansible cannot escalate privileges with fingerprint, so it is necessary to disable this function to run the playbook

```sh
# Disable fingerprint
sudo authselect disable-feature with-fingerprint

# Re-enable fingerprint
sudo authselect enable-feature with-fingerprint
