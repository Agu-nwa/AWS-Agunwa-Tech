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
