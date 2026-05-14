<div align="center">

# ACL View and Export

![Version](https://img.shields.io/badge/version-v1.2-teal)
![Platform](https://img.shields.io/badge/platform-Windows%2010%2F11-lightgrey)
![.NET](https://img.shields.io/badge/.NET-8%20Desktop%20Runtime-purple)
![License](https://img.shields.io/badge/license-MIT-green)

**[🇫🇷 Français](#français) · [🇬🇧 English](#english)**

</div>

---

## Français

### À propos

**ACL View and Export** est un outil Windows gratuit pour **analyser, visualiser et exporter les droits NTFS** d'un dossier et de toute son arborescence. Il affiche les permissions sous forme d'arbre coloré, résout les membres des groupes Active Directory et locaux, et génère des rapports détaillés en Excel, CSV ou PDF.

### Fonctionnalités

- **Scan récursif** des droits NTFS sur les dossiers et fichiers
- **Affichage progressif** : chaque nœud apparaît dès que ses droits sont lus, sans attendre la fin du scan
- **Code couleur** : vert (hérité), rouge (dossier explicite), fuchsia (fichier explicite), violet (inaccessible)
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
- **Logo vectoriel** bouclier + cadenas dans toutes les fenêtres

### Prérequis

| Composant | Version requise |
|---|---|
| Système d'exploitation | Windows 10 v1607+ ou Windows 11 |
| .NET Runtime | [.NET 8 Windows Desktop Runtime (x64)](https://dotnet.microsoft.com/download/dotnet/8.0) |
| Droits | Administrateur (requis pour lire les ACLs NTFS) |

### Installation

1. Télécharger **AclViewerExport-v1.2.msi** dans les [Releases](../../releases/latest)
2. Exécuter le fichier MSI et suivre l'assistant d'installation
3. Lancer **ACL View and Export** depuis le bureau ou le menu Démarrer

> Le MSI installe l'application dans `Program Files`, crée un raccourci bureau et un raccourci dans le menu Démarrer. L'ancienne version est désinstallée automatiquement.

---

## English

### About

**ACL View and Export** is a free Windows tool to **analyze, visualize and export NTFS permissions** from a folder and its entire directory tree. It displays permissions as a color-coded tree, resolves Active Directory and local group members, and generates detailed reports in Excel, CSV or PDF format.

### Features

- **Recursive scan** of NTFS rights on folders and files
- **Progressive display**: each node appears as soon as its permissions are read, without waiting for the scan to finish
- **Color coding**: green (inherited), red (explicit folder), fuchsia (explicit file), violet (inaccessible)
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
- **Vector logo** shield + lock across all windows

### Requirements

| Component | Required version |
|---|---|
| Operating System | Windows 10 v1607+ or Windows 11 |
| .NET Runtime | [.NET 8 Windows Desktop Runtime (x64)](https://dotnet.microsoft.com/download/dotnet/8.0) |
| Rights | Administrator (required to read NTFS ACLs) |

### Installation

1. Download **AclViewerExport-v1.2.msi** from [Releases](../../releases/latest)
2. Run the MSI file and follow the setup wizard
3. Launch **ACL View and Export** from the desktop or Start menu

> The MSI installs the application in `Program Files` and creates shortcuts on the desktop and in the Start menu. The previous version is automatically uninstalled.

---

## Changelog

### v1.2 — Logo vectoriel, couleurs et documentation / Vector logo, colors & documentation

- 🇫🇷 Nouveau logo vectoriel (bouclier + cadenas) dans toutes les fenêtres ; icône exe redessinée en 7 tailles (16→256 px)
- 🇫🇷 Fichiers non hérités : **fuchsia** `#C026D3` · Éléments inaccessibles : **violet** `#7C3AED`
- 🇫🇷 Documentation unifiée en 4 langues (page HTML unique avec sélecteur de drapeaux)
- 🇫🇷 Désinstallation automatique de l'ancienne version lors de la mise à jour
- 🇫🇷 Correction du crash du bouton Documentation
---
- 🇬🇧 New vector logo (shield + lock) across all windows; exe icon redesigned in 7 sizes (16→256 px)
- 🇬🇧 Non-inherited files: **fuchsia** `#C026D3` · Inaccessible items: **violet** `#7C3AED`
- 🇬🇧 Unified documentation in 4 languages (single HTML page with flag switcher)
- 🇬🇧 Automatic uninstallation of previous version on update
- 🇬🇧 Fixed Documentation button crash

### v1.1 — Affichage progressif et filtrage / Progressive display and filtering

- 🇫🇷 Affichage progressif de l'arborescence dès que les droits sont lus
- 🇫🇷 Compteurs mis à jour en temps réel · Filtrage par clic sur un compteur
- 🇫🇷 Icône ⧉ pour copier le chemin dans le presse-papiers
---
- 🇬🇧 Progressive tree display as permissions are read
- 🇬🇧 Real-time counters · Filter by clicking a counter
- 🇬🇧 Copy icon ⧉ to copy the selected path to clipboard

### v1.0 — Version initiale / Initial release

- 🇫🇷 Scan récursif NTFS · Résolution des groupes AD et locaux · Arborescence colorée
- 🇫🇷 Export Excel, CSV et PDF · Chronomètre · Barre de progression · Anti-veille
- 🇫🇷 Vérification des prérequis au démarrage avec actions correctives
---
- 🇬🇧 Recursive NTFS scan · AD and local group resolution · Color-coded tree
- 🇬🇧 Excel, CSV and PDF export · Stopwatch · Progress bar · Keep-awake
- 🇬🇧 Prerequisites check at startup with corrective actions

---

<div align="center">

Développé par **Jérôme MATHIEU** · [Suggérer une amélioration](mailto:webmaster@mathieu-jerome.com) · [Faire un don / Donate](https://paypal.me/mathieujerome)

</div>
