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


**Un générateur de visages moderne pour les newgens de Football Manager 26.**

Ceci est une réécriture complète du [NewGAN-Manager](https://github.com/Maradonna90/NewGAN-Manager) original de Maradonna90, reconstruit de zéro en utilisant **Tauri + Svelte 5** pour de meilleures performances et une interface moderne.

<p align="center">
  <img src="assets/screenshot-fr.png" alt="NewGAN Manager 26 Screenshot" width="600">
</p>

---

## 🎮 Fonctionnalités

- **8 Langues** : Anglais, Français, Allemand, Espagnol, Italien, Coréen, Chinois, Ukrainien
- **Interface Moderne** : Interface sombre avec un design épuré
- **Léger** : Construit avec Tauri (Rust + WebView) au lieu d'Electron
- **Validation Intelligente** : Le bouton de génération reste désactivé tant qu'un fichier RTF valide et un dossier d'images ne sont pas sélectionnés
- **3 Modes** : Générer (Generate), Préserver (Preserve), Écraser (Overwrite)

---

## 📥 Installation

### Windows
1. Téléchargez le dernier `.exe` (portable) depuis les [Releases](https://github.com/Lib-LOCALE/NewGAN-Manager-26/releases)
2. Lancez l'application
3. Déplacez les dossiers `views/` et `filters/` dans votre dossier utilisateur Football Manager :
   ```
   Documents\Sports Interactive\Football Manager 2026\
   ```
3. Lancez NewGAN Manager 26

### Linux
1. Téléchargez le `.AppImage` depuis les [Releases](https://github.com/Lib-LOCALE/NewGAN-Manager-26/releases)
2. Pour AppImage : `chmod +x *.AppImage` puis lancez-le
3. Déplacez les dossiers `views/` et `filters/` dans votre dossier utilisateur Football Manager :
   ```
   ~/.local/share/Sports Interactive/Football Manager 2026/
   ```
4. Lancez NewGAN Manager 26

---

## 🚀 Utilisation

### Prérequis
- Utilisez **English (UK)** comme langue dans FM (les autres langues peuvent avoir des codes pays différents)
- Utilisez le **thème par défaut de FM** (les thèmes personnalisés peuvent utiliser des drapeaux au lieu des codes pays)

### Étapes
1. Dans Football Manager, allez sur une vue de recherche de joueurs ou d'effectif
2. Sélectionnez tous les joueurs (Ctrl+A)
3. Clic droit → **Imprimer l'écran** (Export to Web Page) → Sauvegarder en `.rtf`
3. Ouvrez NewGAN Manager 26
4. Sélectionnez le fichier `.rtf` exporté
6. Sélectionnez votre dossier de visages (organisé par dossiers d'ethnies)
7. Choisissez un mode :
   - **Generate** : Assigne des visages aux joueurs qui n'en ont pas
   - **Preserve** : Garde les assignations existantes, n'ajoute que les nouveaux
   - **Overwrite** : Remplace toutes les assignations de visages existantes
8. Cliquez sur **GENERATE FACES**

---

## 👥 Crédits

### NewGAN-Manager Original
- **[Maradonna](https://github.com/Maradonna90)** : Créateur & Développeur Principal
- **Samaroy** : Coordination, Génération d'images
- **[HRiddick](https://sortitoutsi.net/user/profile/137954)** : Nettoyage d'images
- **[Krysler76](https://community.sigames.com/profile/157461-krysler76/)** : Hacking des vues FM
- **Ayal, Zealand, ZeBurgs** : Génération d'images

### NewGAN Manager 26
- **[Lib-LOCALE](https://github.com/Lib-LOCALE)** : Réécriture avec Tauri + Svelte 5

---

## 📄 Licence

Distribué sous la licence publique générale GNU v3.0. Voir `LICENSE` pour plus d'informations.

---

## 🐛 Dépannage

Si vous rencontrez des problèmes, merci d'[ouvrir une issue](https://github.com/Lib-LOCALE/NewGAN-Manager-26/issues) avec :
- Votre système d'exploitation
- Les étapes pour reproduire le problème
- Tout message d'erreur ou capture d'écran

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


