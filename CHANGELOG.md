# 📋 Frameflow - Changelog

All notable changes to Frameflow will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Planned
- Système de mise à jour automatique complet
- Support multi-langues (FR/EN)
- Templates de tutoriels prédéfinis
- Export vers autres formats (PDF, HTML)

---

## [1.8.1] - 2025-09-25

### 🆕 Added
- **Système de diagnostic complet** avec export des logs et informations système
- **Menu Help → Diagnostic Information** pour le support technique
- **Export diagnostic** en fichier texte ou archive ZIP
- **Préparation système de mise à jour** automatique
- **Validation sécurisée** des domaines et fichiers

### 🐛 Fixed
- **Correction majeure changement de thème** - tous les éléments UI se mettent à jour
- **Liste des étapes** reste maintenant cohérente lors du changement de thème
- **Styles CSS complets** pour le thème clair avec couleurs explicites
- **Mise à jour forcée** de tous les widgets lors du changement de thème
- **Gestion d'erreurs** améliorée dans tous les composants

### ⚡ Improved
- **Performance générale** optimisée
- **Interface utilisateur** plus fluide et réactive
- **Stabilité** renforcée dans tous les modules
- **Documentation** technique complète
- **Architecture** préparée pour les futures fonctionnalités

### 🔧 Technical
- Refactoring du système de thèmes
- Amélioration de la gestion des erreurs
- Optimisation du code de l'interface utilisateur
- Préparation de l'infrastructure de mise à jour

---

## [1.8.0] - 2025-09-20

### 🆕 Added
- **Génération Markdown complètement redessinée** avec format amélioré
- **Générateur markdown centralisé** avec structure hiérarchique
- **Format professionnel** compatible Wiki.js
- **Listes numérotées automatiques** (1. 2. 3.) pour les descriptions d'étapes
- **Mode fenêtre maximisée** automatique pour l'éditeur d'images

### 🐛 Fixed
- **Ordre des boutons** corrigé dans l'éditeur d'images
- **Système de coordonnées** fiabilisé avec coordonnées normalisées
- **Couleur du label mode de capture** s'adapte maintenant au thème

### ⚡ Improved
- **Format de tutoriel** professionnel respectant les standards Wiki.js
- **Maximisation de fenêtre** robuste avec géométrie de secours
- **Placeholder des descriptions** amélioré avec explication des listes numérotées

### 🧹 Maintenance
- **Nettoyage** des fichiers de développement/test
- **Structure projet** plus propre et organisée

---

## [1.7.0] - 2025-09-15

### 🆕 Added
- **Architecture MVC moderne** avec adaptateurs
- **Gestion des zones d'effets** refactorisée et simplifiée
- **Système de métadonnées** JSON robuste
- **Drag & drop des étapes** avec réorganisation visuelle
- **Menu contextuel** complet pour la gestion des étapes

### ⚡ Improved
- **Interface utilisateur** moderne avec PyQt6
- **Persistance des tutoriels** en cours
- **Performance** générale optimisée

---

## [1.6.0] - 2025-09-10

### 🆕 Added
- **Capture automatique/manuelle** avec raccourci F9
- **Détection et sélection de fenêtres** avec thumbnails
- **Édition d'images** (flou, surbrillance)
- **Génération automatique** de markdown
- **Support thèmes** sombre/clair

### 🐛 Fixed
- Stabilité générale améliorée
- Gestion mémoire optimisée

---

## [1.5.0] - 2025-09-05

### 🆕 Added
- Interface PyQt6 moderne
- Système de capture d'écran de base
- Export markdown basique

---

## Version Numbering

Frameflow utilise le [Semantic Versioning](https://semver.org/) :

- **MAJOR** (X.0.0) : Changements incompatibles avec les versions précédentes
- **MINOR** (0.X.0) : Nouvelles fonctionnalités compatibles
- **PATCH** (0.0.X) : Corrections de bugs compatibles

### Version Tags
- **Alpha** : Version de développement interne
- **Beta** : Version de test public
- **RC** : Release Candidate (pré-release)
- **Stable** : Version de production

---

## Support

Pour signaler un bug ou demander une fonctionnalité :
1. Utilisez **Help → Diagnostic Information** pour exporter les informations système
2. Créez un rapport détaillé avec les étapes de reproduction
3. Incluez votre version de Frameflow et Windows

---

**Frameflow** - Professional Tutorial Creator
Développé avec ❤️ par Andorrann
