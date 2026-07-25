# DNS Troubleshooting

## Project Overview

This document describes the DNS troubleshooting process performed while configuring Active Directory in a Windows Server 2022 home lab.

## Environment

- Windows Server 2022
- Active Directory Domain Services
- Domain: company.local
- Domain Controller: DC01

## Problem

During domain verification, the following error occurred:

```
*** Can't find _ldap._tcp.dc._msdcs.company.local: Non-existent domain
```

The DNS server also reported:

```
Default Server: Unknown
```

## Troubleshooting Steps

- Verified IPv4 configuration
- Confirmed DNS server IP address
- Verified Active Directory installation
- Confirmed DNS role installation
- Restarted Netlogon service
- Verified SRV records
- Tested name resolution using nslookup
- Confirmed domain controller registration

## Resolution

DNS records successfully registered.

Confirmed successful domain authentication:

```
Welcome to company.local
```

## Skills Demonstrated

- DNS troubleshooting
- Active Directory diagnostics
- Command-line troubleshooting
- Windows Server administration
