<p align="center">
  <img src="src-tauri/icons/icon.png" alt="NewGAN Manager 26" width="128">
</p>

<h1 align="center">NewGAN Manager 26</h1>

<p align="center">
  <strong>Experimental Tauri/Svelte rewrite of NewGAN Manager for Football Manager 26</strong>
</p>

<p align="center">
  <a href="README.cn.md"><img src="https://hatscripts.github.io/circle-flags/flags/cn.svg" width="28" alt="Chinese"></a>&nbsp;
  <a href="README.kr.md"><img src="https://hatscripts.github.io/circle-flags/flags/kr.svg" width="28" alt="Korean"></a>&nbsp;
  <a href="README.da.md"><img src="https://hatscripts.github.io/circle-flags/flags/dk.svg" width="28" alt="Danish"></a>&nbsp;
  <a href="README.de.md"><img src="https://hatscripts.github.io/circle-flags/flags/de.svg" width="28" alt="German"></a>&nbsp;
  <a href="README.el.md"><img src="https://hatscripts.github.io/circle-flags/flags/gr.svg" width="28" alt="Greek"></a>&nbsp;
  <a href="README.md"><img src="https://hatscripts.github.io/circle-flags/flags/gb.svg" width="28" alt="English"></a>&nbsp;
  <a href="README.es.md"><img src="https://hatscripts.github.io/circle-flags/flags/es.svg" width="28" alt="Spanish"></a>&nbsp;
  <a href="README.fr.md"><img src="https://hatscripts.github.io/circle-flags/flags/fr.svg" width="28" alt="French"></a>&nbsp;
  <a href="README.it.md"><img src="https://hatscripts.github.io/circle-flags/flags/it.svg" width="28" alt="Italian"></a>&nbsp;
  <a href="README.nl.md"><img src="https://hatscripts.github.io/circle-flags/flags/nl.svg" width="28" alt="Dutch"></a>&nbsp;
  <a href="README.pl.md"><img src="https://hatscripts.github.io/circle-flags/flags/pl.svg" width="28" alt="Polish"></a>&nbsp;
  <a href="README.pt.md"><img src="https://hatscripts.github.io/circle-flags/flags/pt.svg" width="28" alt="Portuguese"></a>&nbsp;
  <a href="README.sv.md"><img src="https://hatscripts.github.io/circle-flags/flags/se.svg" width="28" alt="Swedish"></a>&nbsp;
  <a href="README.ua.md"><img src="https://hatscripts.github.io/circle-flags/flags/ua.svg" width="28" alt="Ukrainian"></a>
</p>

---

> **Project status**
>
> NewGAN Manager 26 is currently paused because Football Manager 26 changed the data export workflow required to retrieve player IDs. The repository remains useful as a Tauri/Svelte desktop rewrite, UI prototype, localization example, and release-packaging project.

![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Tauri](https://img.shields.io/badge/Tauri-24C8D8?style=for-the-badge&logo=tauri&logoColor=white)
![Svelte](https://img.shields.io/badge/Svelte-FF3E00?style=for-the-badge&logo=svelte&logoColor=white)

## Overview

This project is a rewrite of the original [NewGAN-Manager](https://github.com/Maradonna90/NewGAN-Manager), rebuilt with Tauri, Svelte 5, and TypeScript.

The goal was to explore a lighter desktop architecture than Electron, improve the UI, and provide multilingual documentation and packaging for Windows and Linux.

<p align="center">
  <img src="assets/screenshot-en.png" alt="NewGAN Manager 26 screenshot" width="600">
</p>

## Features Implemented

- Tauri desktop application using Rust and WebView
- Svelte 5 user interface
- Multilingual documentation and UI support
- File and directory selection workflows
- Smart validation before generation actions
- Windows and Linux release packaging
- SHA256 checksums and GitHub release attestations

## Current Limitation

Football Manager 26 removed the export workflow previously used to extract player IDs. Because that upstream data source is unavailable, the end-to-end face generation workflow is paused.

This limitation is documented here so users and recruiters can understand the project state without mistaking it for an abandoned or broken application.

## Technology Stack

- Svelte 5 and TypeScript
- Tauri and Rust
- Vite
- svelte-i18n
- GitHub Actions release workflow

## Installation

Releases are available for review and testing:

[NewGAN Manager 26 releases](https://github.com/Lib-LOCALE/NewGAN-Manager-26/releases/latest)

Because the FM26 data export dependency is currently unavailable, this project should be treated as a paused experimental rewrite rather than a production-ready tool.

## Security Verification

Release artifacts include SHA256 checksums and GitHub attestations.

```bash
gh attestation verify <downloaded-file> --owner Lib-LOCALE
```

## Credits

Original project:

- [Maradonna](https://github.com/Maradonna90): creator and lead developer of the original NewGAN-Manager
- Samaroy: coordination and image generation
- [HRiddick](https://sortitoutsi.net/user/profile/137954): image cleaning
- [Krysler76](https://community.sigames.com/profile/157461-krysler76/): FM view research
- Ayal, Zealand, ZeBurgs: image generation

FM26 rewrite:

- [Lib-LOCALE](https://github.com/Lib-LOCALE): Tauri/Svelte rewrite and multilingual packaging

## License

Distributed under the GNU General Public License v3.0. See [LICENSE](LICENSE) for details.

