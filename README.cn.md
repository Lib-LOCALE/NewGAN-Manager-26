<p align="center">
  <img src="src-tauri/icons/icon.png" alt="NewGAN Manager 26" width="128">
</p>

<h1 align="center">NewGAN Manager 26</h1>

<h4 align="center">📖 Read in your language</h4>

<p align="center">
  <a href="README.cn.md"><img src="https://hatscripts.github.io/circle-flags/flags/cn.svg" width="32" alt="简体中文"></a>&nbsp;
  <a href="README.kr.md"><img src="https://hatscripts.github.io/circle-flags/flags/kr.svg" width="32" alt="한국어"></a>&nbsp;
  <a href="README.da.md"><img src="https://hatscripts.github.io/circle-flags/flags/dk.svg" width="32" alt="Dansk"></a>&nbsp;
  <a href="README.de.md"><img src="https://hatscripts.github.io/circle-flags/flags/de.svg" width="32" alt="Deutsch"></a>&nbsp;
  <a href="README.el.md"><img src="https://hatscripts.github.io/circle-flags/flags/gr.svg" width="32" alt="Ελληνικά"></a>&nbsp;
  <a href="README.md"><img src="https://hatscripts.github.io/circle-flags/flags/gb.svg" width="32" alt="English"></a>&nbsp;
  <a href="README.es.md"><img src="https://hatscripts.github.io/circle-flags/flags/es.svg" width="32" alt="Español"></a>&nbsp;
  <a href="README.fr.md"><img src="https://hatscripts.github.io/circle-flags/flags/fr.svg" width="32" alt="Français"></a>&nbsp;
  <a href="README.it.md"><img src="https://hatscripts.github.io/circle-flags/flags/it.svg" width="32" alt="Italiano"></a>&nbsp;
  <a href="README.nl.md"><img src="https://hatscripts.github.io/circle-flags/flags/nl.svg" width="32" alt="Nederlands"></a>&nbsp;
  <a href="README.pl.md"><img src="https://hatscripts.github.io/circle-flags/flags/pl.svg" width="32" alt="Polski"></a>&nbsp;
  <a href="README.pt.md"><img src="https://hatscripts.github.io/circle-flags/flags/pt.svg" width="32" alt="Português"></a>&nbsp;
  <a href="README.sv.md"><img src="https://hatscripts.github.io/circle-flags/flags/se.svg" width="32" alt="Svenska"></a>&nbsp;
  <a href="README.ua.md"><img src="https://hatscripts.github.io/circle-flags/flags/ua.svg" width="32" alt="Українська"></a>
</p>

---

# NewGAN Manager - FM26 Edition (Fork)

> ⚠️ **PROJECT STATUS: PAUSED / WAITING FOR EXPORT WORKFLOW** ⚠️
>
> **English:** The end-to-end generation workflow is currently **paused for Football Manager 26** because the transition to the Unity Engine removed the "Print Screen" (Ctrl+P) data export feature, which is required to extract Player IDs.
>
> **Français :** Actuellement, cet outil n'est **PAS fonctionnel sur Football Manager 26**. Le passage au moteur Unity a supprimé la fonctionnalité d'export de données (Ctrl+P), indispensable pour récupérer les IDs des joueurs.

---
![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Tauri](https://img.shields.io/badge/Tauri-24C8D8?style=for-the-badge&logo=tauri&logoColor=white)
![Svelte](https://img.shields.io/badge/Svelte-FF3E00?style=for-the-badge&logo=svelte&logoColor=white)

![SHA256](https://img.shields.io/badge/SHA256-Verified-green?style=flat-square&logo=checkmarx)
![SLSA](https://img.shields.io/badge/SLSA-Attested-blue?style=flat-square&logo=github)
![GitHub Attestations](https://img.shields.io/badge/Attestations-Signed-purple?style=flat-square&logo=sigstore)


**Football Manager 26 新生球员的现代化面孔生成器。**

这是对 Maradonna90 原版 [NewGAN-Manager](https://github.com/Maradonna90/NewGAN-Manager) 的完全重写，使用 **Tauri + Svelte 5** 从头重建，以获得更好的性能和现代化的用户界面。

<p align="center">
  <img src="assets/screenshot-cn.png" alt="NewGAN Manager 26 Screenshot" width="600">
</p>

---

## 🎮 功能特性

- **8种语言**：英语、法语、德语、西班牙语、意大利语、韩语、中文、乌克兰语
- **现代化界面**：简洁设计的深色界面
- **轻量级**：使用 Tauri (Rust + WebView) 而非 Electron 构建
- **智能验证**：在选择有效的 RTF 文件和图像文件夹之前，生成按钮保持禁用状态
- **3种模式**：生成 (Generate)、保留 (Preserve)、覆盖 (Overwrite)

---

## 📥 安装

### Windows
1. 从 [Releases](https://github.com/Lib-LOCALE/NewGAN-Manager-26/releases) 下载最新的 `.exe`（便携版）或 `.msi` 安装程序
2. 运行应用程序
3. 将 `views/` 和 `filters/` 文件夹移动到您的 Football Manager 用户文件夹：
   ```
   Documents\Sports Interactive\Football Manager 2026\
   ```
3. 运行 NewGAN Manager 26

### Linux
1. 从 [Releases](https://github.com/Lib-LOCALE/NewGAN-Manager-26/releases) 下载 `.AppImage` 或 `.deb`
2. AppImage：`chmod +x *.AppImage` 然后运行
3. 将 `views/` 和 `filters/` 文件夹移动到您的 Football Manager 用户文件夹：
   ```
   ~/.local/share/Sports Interactive/Football Manager 2026/
   ```
4. 运行 NewGAN Manager 26

---

## 🚀 使用方法

### 前提条件
- 使用 **English (UK)** 作为 FM 语言（其他语言可能有不同的国家代码）
- 使用 **FM 默认皮肤**（自定义皮肤可能使用国旗而不是国家代码）

### 步骤
1. 在 Football Manager 中，进入球员搜索/球队视图
2. 选择所有球员 (Ctrl+A)
3. 右键点击 → **导出为网页** → 保存为 `.rtf`
3. 打开 NewGAN Manager 26
4. 选择导出的 `.rtf` 文件
6. 选择您的面孔目录（按种族文件夹组织）
7. 选择一个模式：
   - **Generate**：为没有现有面孔的球员分配面孔
   - **Preserve**：保留现有映射，只为新球员分配
   - **Overwrite**：替换所有现有的面孔映射
8. 点击 **GENERATE FACES**

---

## 👥 致谢

### 原版 NewGAN-Manager
- **[Maradonna](https://github.com/Maradonna90)**：创建者和首席开发者
- **Samaroy**：协调、图像生成
- **[HRiddick](https://sortitoutsi.net/user/profile/137954)**：图像清理
- **[Krysler76](https://community.sigames.com/profile/157461-krysler76/)**：FM 视图破解
- **Ayal, Zealand, ZeBurgs**：图像生成

### NewGAN Manager 26
- **[Lib-LOCALE](https://github.com/Lib-LOCALE)**：使用 Tauri + Svelte 5 重写

---

## 📄 许可证

根据 GNU 通用公共许可证 v3.0 分发。有关更多信息，请参阅 `LICENSE`。

---

## 🐛 故障排除

如果您遇到问题，请[提交 issue](https://github.com/Lib-LOCALE/NewGAN-Manager-26/issues)，包括：
- 您的操作系统
- 重现步骤
- 任何错误消息或截图

---

<p align="center">
  <a href="https://liberapay.com/TonyBoySUPER/donate">
    <img alt="Donate using Liberapay" src="https://liberapay.com/assets/widgets/donate.svg">
  </a>
</p>



## 🔒 Security Verification
All releases are cryptographically signed and verified:
- **SHA256 Checksums**: Compare with checksums_windows.txt / checksums_linux.txt
- **GitHub Attestations**: Verify build provenance with:
`ash
gh attestation verify <downloaded-file> --owner Lib-LOCALE
`


