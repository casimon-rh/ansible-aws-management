# ansible-aws-management
Simple start 🟩, stop 🟥, check 🔍 ec2 info with tag ```name: kubernetes``` ☸️

## Vault 🔐

```bash
ansible-vault create aws_keys.yml
# aws_access_key: "{{my_access_key}}"
# aws_secret_key: "{{my_secret_key}}"
```

## Run 🏃‍♂️

```bash
ansible-playbook check.yaml --ask-vault-password
ansible-playbook start.yaml --ask-vault-password
ansible-playbook stop.yaml --ask-vault-password
```
