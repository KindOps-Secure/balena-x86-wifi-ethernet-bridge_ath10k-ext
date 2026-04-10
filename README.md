# balena-x86-wifi-ethernet-bridge_ath10k-ext
# x86 ath10k firmware hostapp extension

This repository builds a **BalenaOS hostapp extension** that injects
`firmware-atheros` (ath10k firmware) into the host OS for
`genericx86-64-ext` devices (Sophos XG, Protectli, Qotom, etc.).

## Prerequisites

- Balena CLI logged in (`balena login`)
- A BalenaCloud fleet running `genericx86-64-ext` BalenaOS
- The BalenaOS version of that fleet (e.g. `2.126.0`)

Edit `Dockerfile.template` and set:

```dockerfile
FROM balena-os/genericx86-64-ext:<BALENAOS_VERSION>
