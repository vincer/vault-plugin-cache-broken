Reproduction for https://github.com/jhaals/ansible-vault/issues/61

## Setup

`ansible-galaxy install --roles-path plugins --force --role-file requirements-plugins.yaml`

## Run

`ansible-playbook --forks=1 -i localhost, playbook.yml`

## Result

No cache hits even though we're reading the same Vault key everytime.
