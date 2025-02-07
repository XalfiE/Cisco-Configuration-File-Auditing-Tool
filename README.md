This executable reads a Cisco IOS configuration file and checks for compliance with a set of recommended security best practices derived mostly from the CIS Cisco IOS 12 Benchmark v4.0.0.

Checks include (but are not limited to):
  - Disabling IP domain lookup
  - Configuring an enable secret and username secret
  - Enabling AAA new-model and AAA authentication for login and enable
  - Ensuring local user privilege is set to 1 (i.e. no high‑privilege default accounts)
  - Ensuring VTY, console, and TTY exec‑timeout values are no more than 10 minutes
  - Disabling CDP, BOOTP, DHCP, IP identd, source routing, and PAD service
  - Enabling TCP keepalives (in and out)
  - Configuring SSH timeout, authentication-retries, and forcing SSH version 2
  - Configuring a domain name and generating RSA keys with modulus ≥ 2048
  - Configuring logging (on, buffered, console, syslog host, trap level, timestamps, source‑interface)
  - Configuring NTP servers
  - Checking that SNMP community strings are not set to insecure default values
  - Configuring banner motd, login and exec banners
  - Checking for generic or default usernames (e.g. admin, cisco, test, demo, guest, default, administrator)
