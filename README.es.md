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


**Un generador de caras moderno para los newgens de Football Manager 26.**

Esta es una reescritura completa del [NewGAN-Manager](https://github.com/Maradonna90/NewGAN-Manager) original de Maradonna90, reconstruido desde cero usando **Tauri + Svelte 5** para un mejor rendimiento y una interfaz moderna.

<p align="center">
  <img src="assets/screenshot-es.png" alt="NewGAN Manager 26 Screenshot" width="600">
</p>

---

## 🎮 Características

- **8 Idiomas**: Inglés, Francés, Alemán, Español, Italiano, Coreano, Chino, Ucraniano
- **Interfaz Moderna**: Interfaz oscura con diseño limpio
- **Ligero**: Construido con Tauri (Rust + WebView) en lugar de Electron
- **Validación Inteligente**: El botón de generación permanece desactivado hasta que se seleccione un archivo RTF válido y una carpeta de imágenes
- **3 Modos**: Generar (Generate), Preservar (Preserve), Sobrescribir (Overwrite)

---

## 📥 Instalación

### Windows
1. Descarga el último `.exe` (portable) desde [Releases](https://github.com/Lib-LOCALE/NewGAN-Manager-26/releases)
2. Ejecuta la aplicación
3. Mueve las carpetas `views/` y `filters/` a tu carpeta de usuario de Football Manager:
   ```
   Documents\Sports Interactive\Football Manager 2026\
   ```
3. Ejecuta NewGAN Manager 26

### Linux
1. Descarga el `.AppImage` desde [Releases](https://github.com/Lib-LOCALE/NewGAN-Manager-26/releases)
2. Para AppImage: `chmod +x *.AppImage` y luego ejecútalo
3. Mueve las carpetas `views/` y `filters/` a tu carpeta de usuario de Football Manager:
   ```
   ~/.local/share/Sports Interactive/Football Manager 2026/
   ```
4. Ejecuta NewGAN Manager 26

---

## 🚀 Uso

### Requisitos previos
- Usa **English (UK)** como idioma en FM (otros idiomas pueden tener códigos de país diferentes)
- Usa el **skin por defecto de FM** (los skins personalizados pueden usar banderas en lugar de códigos de país)

### Pasos
1. En Football Manager, ve a una vista de búsqueda de jugadores o plantilla
2. Selecciona todos los jugadores (Ctrl+A)
3. Clic derecho → **Exportar a página web** → Guardar como `.rtf`
3. Abre NewGAN Manager 26
4. Selecciona el archivo `.rtf` exportado
6. Selecciona tu carpeta de caras (organizada por carpetas de etnicidades)
7. Elige un modo:
   - **Generate**: Asigna caras a jugadores sin caras existentes
   - **Preserve**: Mantiene las asignaciones existentes, solo asigna a nuevos jugadores
   - **Overwrite**: Reemplaza todas las asignaciones de caras existentes
8. Haz clic en **GENERATE FACES**

---

## 👥 Créditos

### NewGAN-Manager Original
- **[Maradonna](https://github.com/Maradonna90)**: Creador y Desarrollador Principal
- **Samaroy**: Coordinación, Generación de imágenes
- **[HRiddick](https://sortitoutsi.net/user/profile/137954)**: Limpieza de imágenes
- **[Krysler76](https://community.sigames.com/profile/157461-krysler76/)**: Hacking de vistas FM
- **Ayal, Zealand, ZeBurgs**: Generación de imágenes

### NewGAN Manager 26
- **[Lib-LOCALE](https://github.com/Lib-LOCALE)**: Reescritura con Tauri + Svelte 5

---

## 📄 Licencia

Distribuido bajo la Licencia Pública General GNU v3.0. Consulte `LICENSE` para más información.

---

## 🐛 Solución de problemas

Si encuentras problemas, por favor [abre un issue](https://github.com/Lib-LOCALE/NewGAN-Manager-26/issues) con:
- Tu sistema operativo
- Pasos para reproducir el problema
- Cualquier mensaje de error o captura de pantalla

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


