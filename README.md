<div align="center">

# ACL View and Export

![Version](https://img.shields.io/badge/version-v1.1-blue)
![Platform](https://img.shields.io/badge/platform-Windows%2010%2F11-lightgrey)
![.NET](https://img.shields.io/badge/.NET-8%20Desktop%20Runtime-purple)
![License](https://img.shields.io/badge/license-Freeware-green)

**[🇫🇷 Français](#français) · [🇬🇧 English](#english)**

</div>

---

## Français

### À propos

**ACL View and Export** est un outil Windows gratuit pour **analyser, visualiser et exporter les droits NTFS** d'un dossier et de toute son arborescence. Il affiche les permissions sous forme d'arbre coloré, résout les membres des groupes Active Directory et locaux, et génère des rapports détaillés en Excel, CSV ou PDF.

### Fonctionnalités

- **Scan récursif** des droits NTFS sur les dossiers et fichiers
- **Affichage progressif** : chaque nœud apparaît dès que ses droits sont lus, sans attendre la fin du scan
- **Code couleur** : vert (hérité), rouge (explicite dossier), orange (explicite fichier), bleu (accès refusé)
- **Résolution des groupes** Active Directory et locaux (membres expandés avec protection anti-boucle)
- **Compteurs en temps réel** : dossiers non hérités, fichiers non hérités, éléments inaccessibles — mis à jour pendant le scan
- **Filtrage par compteur** : clic sur un compteur pour n'afficher que les nœuds correspondants, re-clic pour tout réafficher
- **Copie de chemin** : icône ⧉ pour copier le chemin du dossier ou fichier sélectionné
- **Export Excel (.xlsx)** : 2 onglets (ACL + Membres), en-têtes colorées, lignes rouges/jaunes selon les droits
- **Export CSV** : 2 fichiers UTF-8 (ACL + Membres), directement ouvrables dans Excel
- **Export PDF** : rapport soigné par dossier avec résumé statistique et membres résolus
- **Chronomètre de scan** et barre de progression avec pourcentage exact
- **Option anti-veille** pour les scans de longue durée
- **Annulation** du scan à tout moment

### Prérequis

| Composant | Version requise |
|---|---|
| Système d'exploitation | Windows 10 v1607+ ou Windows 11 |
| .NET Runtime | [.NET 8 Windows Desktop Runtime (x64)](https://dotnet.microsoft.com/download/dotnet/8.0) |
| Droits | Administrateur (requis pour lire les ACLs NTFS) |

### Installation

1. Télécharger **AclViewerExport-v1.1.msi** dans les [Releases](../../releases/latest)
2. Exécuter le fichier MSI et suivre l'assistant d'installation
3. Lancer **ACL View and Export** depuis le bureau ou le menu Démarrer

> Le MSI installe l'application dans `Program Files`, crée un raccourci bureau et un raccourci dans le menu Démarrer.

---

## English

### About

**ACL View and Export** is a free Windows tool to **analyze, visualize and export NTFS permissions** from a folder and its entire directory tree. It displays permissions as a color-coded tree, resolves Active Directory and local group members, and generates detailed reports in Excel, CSV or PDF format.

### Features

- **Recursive scan** of NTFS rights on folders and files
- **Progressive display**: each node appears as soon as its permissions are read, without waiting for the scan to finish
- **Color coding**: green (inherited), red (explicit folder), orange (explicit file), dark blue (access denied)
- **Group resolution** for Active Directory and local groups (expanded members with loop protection)
- **Real-time counters**: non-inherited folders, non-inherited files, inaccessible items — updated live during the scan
- **Counter filtering**: click a counter to show only matching nodes, click again to show all
- **Path copy**: ⧉ icon to copy the selected folder or file path to clipboard
- **Excel export (.xlsx)**: 2 tabs (ACL + Members), colored headers, red/yellow rows for explicit rights
- **CSV export**: 2 UTF-8 files (ACL + Members), directly openable in Excel
- **PDF export**: polished per-folder report with statistics and resolved members
- **Scan stopwatch** and progress bar with exact percentage
- **Keep-awake option** for long scans
- **Cancellation** at any time

### Requirements

| Component | Required version |
|---|---|
| Operating System | Windows 10 v1607+ or Windows 11 |
| .NET Runtime | [.NET 8 Windows Desktop Runtime (x64)](https://dotnet.microsoft.com/download/dotnet/8.0) |
| Rights | Administrator (required to read NTFS ACLs) |

### Installation

1. Download **AclViewerExport-v1.1.msi** from [Releases](../../releases/latest)
2. Run the MSI file and follow the setup wizard
3. Launch **ACL View and Export** from the desktop or Start menu

> The MSI installs the application in `Program Files` and creates shortcuts on the desktop and in the Start menu.

---

## Changelog

### v1.1 — Affichage progressif et filtrage des résultats / Progressive display and result filtering

- 🇫🇷 Affichage progressif de l'arborescence : chaque dossier et fichier apparaît dès que ses droits NTFS sont lus
- 🇫🇷 Compteurs (rouge, bleu, orange) mis à jour en temps réel au cours du scan
- 🇫🇷 Filtrage par clic sur un compteur : affiche uniquement les nœuds correspondants et leurs dossiers ancêtres — re-clic pour tout réafficher
- 🇫🇷 Icône ⧉ pour copier le chemin du dossier ou fichier sélectionné dans le presse-papiers
---
- 🇬🇧 Progressive tree display: each folder and file appears as soon as its NTFS rights are read
- 🇬🇧 Counters (red, blue, orange) updated in real time during the scan
- 🇬🇧 Filter by clicking a counter: shows only matching nodes and their ancestor folders — click again to show all
- 🇬🇧 Copy icon ⧉ to copy the selected path to the clipboard

### v1.0 — Version initiale / Initial release

- 🇫🇷 Scan récursif des droits NTFS sur les dossiers et fichiers
- 🇫🇷 Résolution des membres des groupes locaux et Active Directory
- 🇫🇷 Affichage en arborescence avec code couleur
- 🇫🇷 Export Excel (.xlsx), CSV et PDF
- 🇫🇷 Chronomètre, barre de progression, annulation, option anti-veille
- 🇫🇷 Vérification des prérequis au démarrage avec actions correctives
---
- 🇬🇧 Recursive NTFS rights scan on folders and files
- 🇬🇧 Local and Active Directory group member resolution
- 🇬🇧 Color-coded tree view
- 🇬🇧 Excel (.xlsx), CSV and PDF export
- 🇬🇧 Stopwatch, progress bar, cancellation, keep-awake option
- 🇬🇧 Prerequisites check at startup with corrective actions

---

<div align="center">

Développé par **Jérôme MATHIEU** · [Suggérer une amélioration](mailto:webmaster@mathieu-jerome.com) · [Faire un don / Donate](https://paypal.me/mathieujerome)

</div>
