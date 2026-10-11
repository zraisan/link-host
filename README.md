# Link Host

Link Host is the companion to the **Link** Android app. Install it on your computer, scan the code it prints with the app, and your phone reaches the computer's coding agents, terminals, files and desktop over one encrypted SSH connection, with no port forwarding and no VPN to set up.

This repository holds Link Host's releases. **Docs: https://link.docs.razin.ai**

## Install

Linux and macOS:

```sh
curl -fsSL https://link.docs.razin.ai/install.sh | sh
```

Windows (PowerShell):

```powershell
irm https://link.docs.razin.ai/install.ps1 | iex
```

The installers download the release for your computer from this repository's [Releases](https://github.com/zraisan/link-host/releases), check it against the release's `SHA256SUMS`, and install it for your account only. On Linux the installer then prints a QR code: in the Link app, tap **+ → Scan QR code**.

Linux is the complete platform today (QR pairing, every connection mode, the desktop). On macOS and Windows the phone connects through the system's own SSH server; see [macOS and Windows](https://link.docs.razin.ai/docs/macos-windows).

## Releases

Each release has one archive per platform (`linux_x86_64`, `linux_aarch64`, `macos_x86_64`, `macos_arm64`, `windows_x86_64`, `windows_arm64`), `SHA256SUMS`, and the installers. To check a download by hand:

```sh
sha256sum -c SHA256SUMS --ignore-missing
```

## Problems

[Open an issue](https://github.com/zraisan/link-host/issues). For security problems, please don't open a public issue; email the address on the maintainer's GitHub profile instead.
