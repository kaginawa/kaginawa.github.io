## Kaginawa

Kaginawa is a remote maintenance and data collection software designed for IoT gateways.

![](https://raw.githubusercontent.com/kaginawa/kaginawa/master/docs/overview.png)

## Repositories

Core components:

- [kaginawa](https://github.com/kaginawa/kaginawa) - Main program, works on edge devices, servers, local machines, etc
- [kaginawa-server](https://github.com/kaginawa/kaginawa-server) - Server program, works on Heroku and similar PaaS or IaaS

Utilities:

- [kssh](https://github.com/kaginawa/kssh) - SSH-like command-line utility for connecting kaginawa host easily

SDKs:

- [kaginawa-sdk-go](https://github.com/kaginawa/kaginawa-sdk-go) - Kaginawa Server client library for the Go programming language
- [kaginawa-sdk-java](https://github.com/kaginawa/kaginawa-sdk-java) - Kaginawa Server client library for the Java and other JVM languages

## Download

| OS      | Arch       | Download Link                                             | Archive Format | Checksum                                     |
| ------- | ---------- | --------------------------------------------------------- | -------------- | -------------------------------------------- |
| Linux   | amd64      | [kaginawa.linux-x64.bz2](/kaginawa.linux-x64.bz2)         | bzip2          | [sha256](/kaginawa.linux-x64.bz2.sha256)     |
| Linux   | armv5      | [kaginawa.linux-arm5.bz2](/kaginawa.linux-arm5.bz2)       | bzip2          | [sha256](/kaginawa.linux-arm5.bz2.sha256)    |
| Linux   | armv6      | [kaginawa.linux-arm6.bz2](/kaginawa.linux-arm6.bz2)       | bzip2          | [sha256](/kaginawa.linux-arm6.bz2.sha256)    |
| Linux   | armv7      | [kaginawa.linux-arm7.bz2](/kaginawa.linux-arm7.bz2)       | bzip2          | [sha256](/kaginawa.linux-arm7.bz2.sha256)    |
| Linux   | armv8 (64) | [kaginawa.linux-arm8.bz2](/kaginawa.linux-arm8.bz2)       | bzip2          | [sha256](/kaginawa.linux-arm8.bz2.sha256)    |
| Linux   | riscv64    | [kaginawa.linux-riscv64.bz2](/kaginawa.linux-riscv64.bz2) | bzip2          | [sha256](/kaginawa.linux-riscv64.bz2.sha256) |
| MacOS   | amd64      | [kaginawa.macos-x64.bz2](/kaginawa.macos-x64.bz2)         | bzip2          | [sha256](/kaginawa.macos-x64.bz2.sha256)     |
| MacOS   | arm64      | [kaginawa.macos-arm64.bz2](/kaginawa.macos-arm64.bz2)     | bzip2          | [sha256](/kaginawa.macos-arm64.bz2.sha256)   |
| Windows | amd64      | [kaginawa.exe.zip](/kaginawa.exe.zip)                     | zip            | [sha256](/kaginawa.exe.zip.sha256)           |

## FAQ

**What do I need to start using Kaginawa?**

Kaginawa is a client-server model application with three building blocks.

1. Kaginawa program is deployed to the target machine (PCs, laptops, IoT devices, servers, etc.)
2. Kaginawa Server is deployed to the server machine (IaaS, PaaS, on-premis servers, etc.)
3. Standard OpenSSH Server

Kaginawa Server (item 2) and SSH Server (item 3) are separated processes, but each can run on one server.

**I'm using Raspberry Pi. Which binaries work on my board?**

If you use Raspberry Pi 1, Zero (incl. W, WH) or Compute Module (CM1), use armv6 binary.
Otherwise use armv7 binary.

**I'm using NanoPi or similar boards. Which binaries work on my board?**

If you use arm64 operating systems, use armv8 (arm64) binary.
Otherwise use armv7 binary.
