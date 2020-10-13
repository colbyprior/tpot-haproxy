# T-Pot HAProxy
This is an Ansible playbook to deploy a HAProxy config to create a lightweight honepot proxy for T-Pot.

## Testing the playbook from localhost
`ansible-playbook playbook.yml -i inventory.yml --connection=local -l localhost`

## Adding to the inventory
- Add hosts under `prod:` in `inventory.yml`.
- You must update the `honeypot_address` variable to the address of your T-Pot server.
- Add any of the following vars to enable the different listeners:

# List of available listeners
- ssh
- smtp
- http
- https
