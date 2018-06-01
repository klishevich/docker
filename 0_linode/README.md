# Setting Up Linode Server

1. Create New Linode
2. `apt-get update && apt-get upgrade`
3. `hostnamectl set-hostname`
4. Update /etc/hosts
  ```
  127.0.0.1 localhost.localdomain localhost
  203.0.113.10 hostname.example.com hostname
  ```
5. Set timezone `dpkg-reconfigure tzdata` (check: `date`)

## Securing Linode

1. TODO unattended upgrades
2. `adduser mike`
3. `adduser mike sudo`
4. On Linode `mkdir -p ~/.ssh && sudo chmod -R 700 ~/.ssh/`
5. On Mac `scp ~/.ssh/id_rsa.pub mike@deimos.j123.ru:~/.ssh/authorized_keys`
6. /etc/ssh/sshd_config
  * PermitRootLogin no
  * PasswordAuthentication no
  * AddressFamily inet
7. sudo systemctl restart sshd
