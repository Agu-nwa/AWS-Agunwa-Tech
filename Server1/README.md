## ⚙️ 1. Login Ubuntu

### Command
```bash
ssh -i ~/Documents/port.pem ubuntu@100.27.xxx.xxx

Welcome to Ubuntu 26.04 LTS (GNU/Linux 7.0.0-1006-aws x86_64)

 * Documentation:  https://docs.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/pro

 System information as of Sat Jun 20 17:45:58 UTC 2026

  System load:  0.0               Temperature:           -273.1 C
  Usage of /:   30.5% of 6.61GB   Processes:             115
  Memory usage: 25%               Users logged in:       0
  Swap usage:   0%                IPv4 address for ens5: 172.31.29.182

Expanded Security Maintenance for Applications is not enabled.

0 updates can be applied immediately.

Enable ESM Apps to receive additional future security updates.
See https://ubuntu.com/esm or run: sudo pro status


The list of available updates is more than a week old.
To check for new updates run: sudo apt update


The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

## ⚙️ 1. Update System Packages

### Command
```bash
sudo apt update

Hit:1 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute InRelease
Get:2 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates InRelease [137 kB]
Get:3 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-backports InRelease [136 kB]
Get:4 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute/universe amd64v3 Packages [16.3 MB]
Get:5 http://security.ubuntu.com/ubuntu resolute-security InRelease [137 kB]
Get:6 http://security.ubuntu.com/ubuntu resolute-security/main amd64v3 Packages [216 kB]
Get:7 http://security.ubuntu.com/ubuntu resolute-security/main Translation-en [59.2 kB]
Get:8 http://security.ubuntu.com/ubuntu resolute-security/main amd64 Components [31.1 kB]
Get:9 http://security.ubuntu.com/ubuntu resolute-security/main amd64 c-n-f Metadata [3592 B]
Get:10 http://security.ubuntu.com/ubuntu resolute-security/universe amd64v3 Packages [125 kB]
Get:11 http://security.ubuntu.com/ubuntu resolute-security/universe Translation-en [38.7 kB]
Get:12 http://security.ubuntu.com/ubuntu resolute-security/universe amd64 Components [43.1 kB]      
Get:13 http://security.ubuntu.com/ubuntu resolute-security/universe amd64 c-n-f Metadata [3264 B]
Get:14 http://security.ubuntu.com/ubuntu resolute-security/multiverse amd64 Components [212 B]
Get:15 http://security.ubuntu.com/ubuntu resolute-security/multiverse amd64 c-n-f Metadata [120 B]
Get:16 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute/universe Translation-en [6329 kB]
Get:17 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute/universe amd64 Components [4556 kB]
Get:18 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute/universe amd64 c-n-f Metadata [313 kB]
Get:19 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute/multiverse amd64v3 Packages [291 kB]
Get:20 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute/multiverse Translation-en [127 kB]
Get:21 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute/multiverse amd64 Components [50.0 kB]
Get:22 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute/multiverse amd64 c-n-f Metadata [8276 B]
Get:23 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 Packages [257 kB]
Get:24 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main Translation-en [68.9 kB]
Get:25 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64 Components [49.4 kB]
Get:26 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64 c-n-f Metadata [4400 B]
Get:27 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/universe amd64v3 Packages [150 kB]
Get:28 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/universe Translation-en [47.0 kB]
Get:29 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/universe amd64 Components [62.2 kB]
Get:30 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/universe amd64 c-n-f Metadata [3908 B]
Get:31 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/restricted amd64v3 Packages [208 kB]
Get:32 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/restricted Translation-en [36.1 kB]
Get:33 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/multiverse amd64v3 Packages [3360 B]
Get:34 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/multiverse Translation-en [772 B]
Get:35 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/multiverse amd64 Components [216 B]
Get:36 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/multiverse amd64 c-n-f Metadata [256 B]
Get:37 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-backports/main amd64 Components [212 B]
Get:38 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-backports/main amd64 c-n-f Metadata [112 B]
Get:39 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-backports/universe amd64 Components [216 B]
Get:40 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-backports/universe amd64 c-n-f Metadata [116 B]
Get:41 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-backports/restricted amd64 Components [216 B]
Get:42 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-backports/restricted amd64 c-n-f Metadata [120 B]
Get:43 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-backports/multiverse amd64 Components [216 B]
Get:44 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-backports/multiverse amd64 c-n-f Metadata [120 B]
Fetched 29.8 MB in 4s (7538 kB/s)               
17 packages can be upgraded. Run 'apt list --upgradable' to see them.

## ⚙️ 1. Upgrade System Packages

### Command
```bash
sudo apt upgrade -y

Upgrading:                      
  ca-certificates   libssl3t64  openssl                  python3-distupgrade  telnet  ubuntu-release-upgrader-core  vim         vim-runtime  xxd
  inetutils-telnet  nano        openssl-provider-legacy  rsync                tmux    update-notifier-common        vim-common  vim-tiny

Summary:
  Upgrading: 17, Installing: 0, Removing: 0, Not Upgrading: 0
14 standard LTS security updates
  Download size: 16.5 MB
  Freed space: 36.9 kB

Get:1 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 update-notifier-common all 3.207.1 [212 kB]
Get:2 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 openssl-provider-legacy amd64 3.5.5-1ubuntu3.2 [40.4 kB]
Get:3 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 libssl3t64 amd64 3.5.5-1ubuntu3.2 [2366 kB]
Get:4 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 openssl amd64 3.5.5-1ubuntu3.2 [1243 kB]
Get:5 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 ca-certificates all 20260601~26.04.1 [139 kB]
Get:6 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 vim amd64 2:9.1.2141-1ubuntu4.5 [2071 kB]
Get:7 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 vim-common all 2:9.1.2141-1ubuntu4.5 [494 kB]
Get:8 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 vim-tiny amd64 2:9.1.2141-1ubuntu4.5 [870 kB]
Get:9 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 vim-runtime all 2:9.1.2141-1ubuntu4.5 [7512 kB]
Get:10 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 xxd amd64 2:9.1.2141-1ubuntu4.5 [68.4 kB]
Get:11 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 inetutils-telnet amd64 2:2.7-2ubuntu1.1 [108 kB]
Get:12 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 nano amd64 8.7.1-1ubuntu0.1 [290 kB]
Get:13 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 ubuntu-release-upgrader-core all 1:26.04.22 [24.9 kB]
Get:14 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 python3-distupgrade all 1:26.04.22 [102 kB]
Get:15 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 rsync amd64 3.4.1+ds1-7ubuntu0.3 [447 kB]
Get:16 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 telnet all 0.17+2.7-2ubuntu1.1 [3650 B]
Get:17 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 tmux amd64 3.6a-2ubuntu0.1 [516 kB]
Fetched 16.5 MB in 0s (86.5 MB/s)
Preconfiguring packages ...
(Reading database ... 85303 files and directories currently installed.)
Preparing to unpack .../update-notifier-common_3.207.1_all.deb ...
Unpacking update-notifier-common (3.207.1) over (3.207) ...
Preparing to unpack .../openssl-provider-legacy_3.5.5-1ubuntu3.2_amd64v3.deb ...
Unpacking openssl-provider-legacy (3.5.5-1ubuntu3.2) over (3.5.5-1ubuntu3) ...
Setting up openssl-provider-legacy (3.5.5-1ubuntu3.2) ...
(Reading database ... 85303 files and directories currently installed.)
Preparing to unpack .../libssl3t64_3.5.5-1ubuntu3.2_amd64v3.deb ...
Unpacking libssl3t64:amd64 (3.5.5-1ubuntu3.2) over (3.5.5-1ubuntu3) ...
Setting up libssl3t64:amd64 (3.5.5-1ubuntu3.2) ...
(Reading database ... 85303 files and directories currently installed.)
Preparing to unpack .../00-openssl_3.5.5-1ubuntu3.2_amd64v3.deb ...
Unpacking openssl (3.5.5-1ubuntu3.2) over (3.5.5-1ubuntu3) ...
Preparing to unpack .../01-ca-certificates_20260601~26.04.1_all.deb ...
Unpacking ca-certificates (20260601~26.04.1) over (20260223) ...
Preparing to unpack .../02-vim_2%3a9.1.2141-1ubuntu4.5_amd64v3.deb ...
Unpacking vim (2:9.1.2141-1ubuntu4.5) over (2:9.1.2141-1ubuntu4.2) ...
Preparing to unpack .../03-vim-common_2%3a9.1.2141-1ubuntu4.5_all.deb ...
Unpacking vim-common (2:9.1.2141-1ubuntu4.5) over (2:9.1.2141-1ubuntu4.2) ...
Preparing to unpack .../04-vim-tiny_2%3a9.1.2141-1ubuntu4.5_amd64v3.deb ...
Unpacking vim-tiny (2:9.1.2141-1ubuntu4.5) over (2:9.1.2141-1ubuntu4.2) ...
Preparing to unpack .../05-vim-runtime_2%3a9.1.2141-1ubuntu4.5_all.deb ...
Unpacking vim-runtime (2:9.1.2141-1ubuntu4.5) over (2:9.1.2141-1ubuntu4.2) ...
Preparing to unpack .../06-xxd_2%3a9.1.2141-1ubuntu4.5_amd64v3.deb ...
Unpacking xxd (2:9.1.2141-1ubuntu4.5) over (2:9.1.2141-1ubuntu4.2) ...
Preparing to unpack .../07-inetutils-telnet_2%3a2.7-2ubuntu1.1_amd64v3.deb ...
Unpacking inetutils-telnet (2:2.7-2ubuntu1.1) over (2:2.7-2ubuntu1) ...
Preparing to unpack .../08-nano_8.7.1-1ubuntu0.1_amd64v3.deb ...
Unpacking nano (8.7.1-1ubuntu0.1) over (8.7.1-1) ...
Preparing to unpack .../09-ubuntu-release-upgrader-core_1%3a26.04.22_all.deb ...
Unpacking ubuntu-release-upgrader-core (1:26.04.22) over (1:26.04.18) ...
Preparing to unpack .../10-python3-distupgrade_1%3a26.04.22_all.deb ...
Unpacking python3-distupgrade (1:26.04.22) over (1:26.04.18) ...
Preparing to unpack .../11-rsync_3.4.1+ds1-7ubuntu0.3_amd64v3.deb ...
Unpacking rsync (3.4.1+ds1-7ubuntu0.3) over (3.4.1+ds1-7ubuntu0.2) ...
Preparing to unpack .../12-telnet_0.17+2.7-2ubuntu1.1_all.deb ...
Unpacking telnet (0.17+2.7-2ubuntu1.1) over (0.17+2.7-2ubuntu1) ...
Preparing to unpack .../13-tmux_3.6a-2ubuntu0.1_amd64v3.deb ...
Unpacking tmux (3.6a-2ubuntu0.1) over (3.6a-2) ...
Setting up update-notifier-common (3.207.1) ...
update-notifier-download.service is a disabled or a static unit not running, not starting it.
update-notifier-motd.service is a disabled or a static unit not running, not starting it.
Setting up inetutils-telnet (2:2.7-2ubuntu1.1) ...
Setting up python3-distupgrade (1:26.04.22) ...
Setting up xxd (2:9.1.2141-1ubuntu4.5) ...
Setting up vim-common (2:9.1.2141-1ubuntu4.5) ...
Setting up nano (8.7.1-1ubuntu0.1) ...
Setting up vim-runtime (2:9.1.2141-1ubuntu4.5) ...
Setting up openssl (3.5.5-1ubuntu3.2) ...
Setting up tmux (3.6a-2ubuntu0.1) ...
Setting up rsync (3.4.1+ds1-7ubuntu0.3) ...
rsync.service is a disabled or a static unit not running, not starting it.
Setting up vim (2:9.1.2141-1ubuntu4.5) ...
Setting up telnet (0.17+2.7-2ubuntu1.1) ...
Setting up vim-tiny (2:9.1.2141-1ubuntu4.5) ...
Setting up ca-certificates (20260601~26.04.1) ...
Updating certificates in /etc/ssl/certs...
rehash: warning: skipping ca-certificates.crt, it does not contain exactly one certificate or CRL
2 added, 25 removed; done.
Setting up ubuntu-release-upgrader-core (1:26.04.22) ...
Installing new version of config file /etc/update-manager/release-upgrades ...
Processing triggers for install-info (7.2-5ubuntu2) ...
Processing triggers for libc-bin (2.43-2ubuntu2) ...
Processing triggers for man-db (2.13.1-1build1) ...
Processing triggers for debianutils (5.23.2build1) ...
Processing triggers for ca-certificates (20260601~26.04.1) ...
Updating certificates in /etc/ssl/certs...
0 added, 0 removed; done.
Running hooks in /etc/ca-certificates/update.d...
done.
Scanning processes...                                                                                                                                                                                       
Scanning candidates...                                                                                                                                                                                      
Scanning linux images...                                                                                                                                                                                    

Running kernel seems to be up-to-date.

Restarting services...
 /etc/needrestart/restart.d/systemd-manager
 /etc/needrestart/restart.d/systemd-user
 systemctl restart packagekit.service ssh.service systemd-journald.service systemd-networkd.service systemd-resolved.service systemd-udevd.service udisks2.service

Service restarts being deferred:
 systemctl restart networkd-dispatcher.service
 systemctl restart systemd-logind.service
 systemctl restart unattended-upgrades.service

No containers need to be restarted.

User sessions running outdated binaries:
 ubuntu @ session #1: apt[1468], sshd-session[1165], sudo[1467]
 ubuntu @ user manager: (sd-pam)[1173]

No VM guests are running outdated hypervisor (qemu) binaries on this host.

## ⚙️ 1. Install Nginx

### Command
```bash
sudo apt install nginx -y

Installing:                     
  nginx

Installing dependencies:
  nginx-common

Suggested packages:
  fcgiwrap  nginx-doc  ssl-cert

Summary:
  Upgrading: 0, Installing: 2, Removing: 0, Not Upgrading: 0
  Download size: 664 kB
  Space needed: 1874 kB / 4676 MB available

Get:1 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 nginx-common all 1.28.3-2ubuntu1.5 [37.2 kB]
Get:2 http://us-east-1.ec2.archive.ubuntu.com/ubuntu resolute-updates/main amd64v3 nginx amd64 1.28.3-2ubuntu1.5 [627 kB]
Fetched 664 kB in 0s (15.4 MB/s)
Preconfiguring packages ...
Selecting previously unselected package nginx-common.
(Reading database ... 85280 files and directories currently installed.)
Preparing to unpack .../nginx-common_1.28.3-2ubuntu1.5_all.deb ...
Unpacking nginx-common (1.28.3-2ubuntu1.5) ...
Selecting previously unselected package nginx.
Preparing to unpack .../nginx_1.28.3-2ubuntu1.5_amd64v3.deb ...
Unpacking nginx (1.28.3-2ubuntu1.5) ...
Setting up nginx-common (1.28.3-2ubuntu1.5) ...
Created symlink '/etc/systemd/system/multi-user.target.wants/nginx.service' → '/usr/lib/systemd/system/nginx.service'.
Setting up nginx (1.28.3-2ubuntu1.5) ...
 * Upgrading binary nginx                                                                                                                                                                            [ OK ] 
Processing triggers for man-db (2.13.1-1build1) ...
Processing triggers for ufw (0.36.2-9build1) ...
Scanning processes...                                                                                                                                                                                       
Scanning candidates...                                                                                                                                                                                      
Scanning linux images...                                                                                                                                                                                    

Running kernel seems to be up-to-date.

Restarting services...

Service restarts being deferred:
 systemctl restart networkd-dispatcher.service
 systemctl restart systemd-logind.service
 systemctl restart unattended-upgrades.service

No containers need to be restarted.

User sessions running outdated binaries:
 ubuntu @ session #1: sshd-session[1165]
 ubuntu @ user manager: (sd-pam)[1173]

No VM guests are running outdated hypervisor (qemu) binaries on this host.

## ⚙️ 1. Start Nginx

### Command
```bash
sudo systemctl start nginx

Successfully started nginx

## ⚙️ 1. Enable Auto Restart Nginx 

### Command
```bash
sudo systemctl enable nginx

Synchronizing state of nginx.service with SysV service script with /usr/lib/systemd/systemd-sysv-install.
Executing: /usr/lib/systemd/systemd-sysv-install enable nginx
