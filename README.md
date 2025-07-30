# Ansible Role Certbot

install Certbot

## Role Variables

| group | variable | default | description |
| --- | --- | --- | --- |
| dns | certbot_dns_hetzner | `false` | if Hetzner DNS Authenticator certbot plugin (certbot-dns-hetzner) should be installed |
| dns | certbot_dns_scaleway | `false` | if Scaleway DNS Authenticator certbot plugin (certbot-dns-scaleway) should be installed |
| dns | certbot_dns_digitalocean | `false` | if DigitalOcean DNS Authenticator certbot plugin (certbot-dns-digitalocean) should be installed |
| hook | certbot_deploy_hook | | the deploy-hook script for /etc/letsencrypt/cli.ini |
| pip | certbot_pip_break_system_packages | `true` | the value for [break_system_packages](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/pip_module.html#parameter-break_system_packages) |
