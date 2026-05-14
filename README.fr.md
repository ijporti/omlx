<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="docs/images/icon-rounded-dark.svg" width="140">
    <source media="(prefers-color-scheme: light)" srcset="docs/images/icon-rounded-light.svg" width="140">
    <img alt="oMLX" src="docs/images/icon-rounded-light.svg" width="140">
  </picture>
</p>

<h1 align="center">oMLX</h1>
<p align="center"><b>Inférence LLM, optimisée pour votre Mac</b><br>Batching continu et cache KV à plusieurs niveaux, géré directement depuis votre barre de menus.</p>

<p align="center">
<a href="https://www.buymeacoffee.com/jundot"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" height="40"></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/license-Apache%202.0-blue" alt="License">
  <img src="https://img.shields.io/badge/python-3.10+-green" alt="Python 3.10+">
  <img src="https://img.shields.io/badge/platform-Apple%20Silicon-black?logo=apple" alt="Apple Silicon">
</p>

<p align="center">
  <a href="mailto:junkim.dot@gmail.com">junkim.dot@gmail.com</a> · <a href="https://omlx.ai/me">https://omlx.ai/me</a>
</p>

<p align="center">
  <a href="#installation">Installation</a> ·
  <a href="#démarrage-rapide">Démarrage rapide</a> ·
  <a href="#fonctionnalités">Fonctionnalités</a> ·
  <a href="#modèles">Modèles</a> ·
  <a href="#configuration-cli">Configuration CLI</a> ·
  <a href="https://omlx.ai/benchmarks">Benchmarks</a> ·
  <a href="https://omlx.ai">oMLX.ai</a>
</p>

<p align="center">
  <a href="README.md">English</a> ·
  <a href="README.zh.md">中文</a> ·
  <a href="README.ko.md">한국어</a> ·
  <a href="README.ja.md">日本語</a> ·
  <b>Français</b>
</p>

---

<p align="center">
  <img src="docs/images/omlx_dashboard.png" alt="oMLX Admin Dashboard" width="800">
</p>

> *Chaque serveur LLM que j'ai essayé m'obligeait à choisir entre commodité et contrôle. Je voulais garder des modèles du quotidien en mémoire, permuter automatiquement les plus lourds à la demande, définir des limites de contexte — et tout gérer depuis la barre de menus.*
>
> *oMLX persiste le cache KV sur un niveau chaud en RAM et un niveau froid sur SSD — même quand le contexte change en cours de conversation, tout le contexte passé reste en cache et réutilisable entre les requêtes, rendant les LLM locaux vraiment pratiques pour du vrai travail de code avec des outils comme Claude Code. C'est pour ça que je l'ai construit.*

## Installation

### Application macOS

Téléchargez le `.dmg` depuis les [Releases](https://github.com/jundot/omlx/releases), glissez-le dans Applications, c'est tout. L'application inclut une mise à jour automatique intégrée, les futures mises à jour se font en un clic. À noter que l'application macOS n'installe pas la commande CLI `omlx`. Pour une utilisation en terminal, installez via Homebrew ou depuis les sources.

### Homebrew

```bash
brew tap jundot/omlx https://github.com/jundot/omlx
brew install omlx

# Mettre à jour vers la dernière version
brew upgrade omlx
```
