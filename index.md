## Kaginawa

Kaginawa is a remote maintenance and data collection software designed for IoT gateways.

## Repositories

- [kaginawa](https://github.com/kaginawa/kaginawa) - Main program, works on edge devices, servers, local machines, etc
- [kaginawa-server](https://github.com/kaginawa/kaginawa-server) - Server program, works on Heroku and similar PaaS or IaaS

## Download

| OS      | Arch  | Download Link                                       | Archive Format |
| ------- | ----- | --------------------------------------------------- | -------------- |
| Linux   | amd64 | [kaginawa.linux-x64.bz2](/kaginawa.linux-x64.bz2)   | bzip2          |
| Linux   | armv6 | [kaginawa.linux-arm6.bz2](/kaginawa.linux-arm6.bz2) | bzip2          |
| Linux   | armv7 | [kaginawa.linux-arm7.bz2](/kaginawa.linux-arm7.bz2) | bzip2          |
| MacOS   | amd64 | [kaginawa.macos.bz2](/kaginawa.macos.bz2)           | bzip2          |
| Windows | amd64 | [kaginawa.exe.zip](/kaginawa.exe.zip)               | zip            |

## FAQ

> What do I need to start using Kaginawa?

Kaginawa is a client-server model application with three building blocks.

1. Kaginawa program is deployed to the target machine (PCs, laptops, IoT devices, servers, etc.)
2. Kaginawa Server is deployed to the server machine (IaaS, PaaS, on-premis servers, etc.)
3. Standard OpenSSH Server

Kaginawa Server (item 2) and SSH Server (item 3) are separated processes, but each can run on one server.

> I'm using Raspberry Pi. Which binaries work on my board?

If you use Raspberry Pi 1, Zero (incl. W, WH) or Compute Module (CM1), use armv6 binary.
Otherwise use armv7 binary.
