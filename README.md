# Ansible Role: Utilvo EdgeShield for Apache 2.4 (`apache2` & `httpd`)

Official Ansible role for deploying **[Utilvo EdgeShield](https://utilvo.com/edge-shield)** across **Ubuntu/Debian (`apache2`)** and **RHEL/AlmaLinux/Rocky/cPanel (`httpd`)** server fleets.

- **Interactive Configurator:** [https://utilvo.com/edge-shield](https://utilvo.com/edge-shield)
- **Raw Apache 2.4 Config:** [https://utilvo.com/edge-shield/apache-bot-shield.conf](https://utilvo.com/edge-shield/apache-bot-shield.conf)
- **Live CIDR Feed:** [https://utilvo.com/api/edge-shield/threats?format=cidr](https://utilvo.com/api/edge-shield/threats?format=cidr)

## Tasks Performed

1. Enables `mod_remoteip`, `mod_setenvif`, `mod_authz_core`, and `mod_rewrite`.
2. Deploys `/etc/apache2/conf-available/utilvo-edge-shield.conf` (or `/etc/httpd/conf.d/utilvo-edge-shield.conf`).
3. Validates syntax via `apache2ctl -t` / `httpd -t` before reloading Apache gracefully.

## License

MIT License — [Utilvo Security Research](https://utilvo.com/edge-shield).
