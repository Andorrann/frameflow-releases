# 📋 INSTRUCTIONS - CRÉATION DU REPO FRAMEFLOW-RELEASES

## 🎯 **ÉTAPES POUR CRÉER LE REPOSITORY GITHUB**

### **1. 📁 Préparation des Fichiers**

Tous les fichiers sont prêts dans `docs/frameflow-releases/` :
- ✅ `README.md` - Description du projet
- ✅ `CHANGELOG.md` - Historique des versions
- ✅ `version.json` - Métadonnées de version
- ✅ `LICENSE` - Licence propriétaire
- ✅ `.gitignore` - Fichiers à ignorer

### **2. 🚀 Création du Repository GitHub**

1. **Aller sur GitHub** : https://github.com/new
2. **Nom du repository** : `frameflow-releases`
3. **Description** : `Frameflow - Professional Tutorial Creator - Official Releases`
4. **Visibilité** : **Public** (obligatoire pour l'API)
5. **Initialiser** : ❌ Ne pas cocher "Add a README file"
6. **Cliquer** : "Create repository"

### **3. 📤 Upload des Fichiers**

#### **Option A : Via l'interface GitHub**
1. **Drag & Drop** tous les fichiers du dossier `docs/frameflow-releases/`
2. **Commit message** : `Initial release repository setup`
3. **Commit directly** to main branch

#### **Option B : Via Git (si tu as Git installé)**
```bash
# Dans le dossier docs/frameflow-releases/
git init
git add .
git commit -m "Initial release repository setup"
git branch -M main
git remote add origin https://github.com/andorrann/frameflow-releases.git
git push -u origin main
```

### **4. 📦 Ajouter l'Exécutable**

1. **Copier** `dist/Frameflow_Setup.exe` dans `docs/frameflow-releases/`
2. **Aller** dans le repo GitHub
3. **Releases** → **Create a new release**
4. **Tag version** : `v1.8.1`
5. **Release title** : `Frameflow 1.8.1 Beta`
6. **Description** : Copier depuis `CHANGELOG.md` (section 1.8.1)
7. **Attach files** : 
   - `Frameflow_Setup.exe`
   - `version.json`
8. **Publish release**

### **5. 🧪 Tester l'API**

Vérifier que l'API fonctionne :
```bash
# Tester dans le navigateur ou avec curl
https://api.github.com/repos/andorrann/frameflow-releases/releases/latest
```

Doit retourner les informations de la release v1.8.1.

## 🔧 **UTILISATION DU VERSION MANAGER**

### **📈 Incrémenter une Version**

```bash
# Depuis la racine du projet Frameflow
python utils/version_manager.py --current
# Affiche: Version actuelle: 1.8.1 Beta

python utils/version_manager.py --increment patch --suffix "Beta"
# Nouvelle version: 1.8.2 Beta

python utils/version_manager.py --increment minor --suffix "RC1"
# Nouvelle version: 1.9.0 RC1

python utils/version_manager.py --increment major --suffix "Stable"
# Nouvelle version: 2.0.0 Stable
```

### **📋 Générer version.json**

```bash
# Après avoir compilé l'exe
python utils/version_manager.py --generate-json "dist/Frameflow_Setup.exe"
# Génère version.json avec taille et hash SHA256 corrects
```

### **📝 Générer Notes de Release**

```bash
python utils/version_manager.py --release-notes
# Génère les notes formatées pour GitHub
```

## 🔄 **WORKFLOW DE RELEASE**

### **📅 Processus Complet pour une Nouvelle Version**

1. **Développer** les nouvelles fonctionnalités
2. **Tester** l'application
3. **Incrémenter la version** :
   ```bash
   python utils/version_manager.py --increment patch --changelog "Correction bugs thème"
   ```
4. **Compiler l'exécutable** :
   ```bash
   build.bat
   ```
5. **Générer version.json** :
   ```bash
   python utils/version_manager.py --generate-json "dist/Frameflow_Setup.exe"
   ```
6. **Copier** `Frameflow_Setup.exe` et `version.json` dans `docs/frameflow-releases/`
7. **Créer la release** sur GitHub
8. **Tester** l'API et le téléchargement

## 📊 **STRUCTURE FINALE**

### **Repository frameflow-releases :**
```
frameflow-releases/
├── README.md
├── CHANGELOG.md
├── LICENSE
├── .gitignore
├── version.json (mis à jour à chaque release)
└── Releases/ (créées via GitHub)
    ├── v1.8.1/
    │   ├── Frameflow_Setup.exe
    │   └── version.json
    ├── v1.8.2/
    │   ├── Frameflow_Setup.exe
    │   └── version.json
    └── ...
```

### **API Endpoints Disponibles :**
- `GET /repos/andorrann/frameflow-releases/releases/latest` - Dernière version
- `GET /repos/andorrann/frameflow-releases/releases` - Toutes les versions
- `GET /repos/andorrann/frameflow-releases/releases/tags/v1.8.1` - Version spécifique

## 🎯 **PROCHAINES ÉTAPES**

1. ✅ **Créer le repo** GitHub avec les fichiers fournis
2. ✅ **Publier la première release** v1.8.1
3. ✅ **Tester l'API** GitHub
4. 🔄 **Implémenter le système** de mise à jour dans Frameflow
5. 🚀 **Tester** le processus complet

## 💡 **CONSEILS**

### **🔐 Sécurité**
- Le repo doit être **public** pour l'API (mais pas le code source)
- Les releases sont **signées** par GitHub automatiquement
- Utiliser **HTTPS** uniquement pour les téléchargements

### **📈 Versioning**
- **Patch** (1.8.1 → 1.8.2) : Corrections de bugs
- **Minor** (1.8.x → 1.9.0) : Nouvelles fonctionnalités
- **Major** (1.x.x → 2.0.0) : Changements incompatibles

### **🏷️ Tags de Version**
- **Beta** : Version de test public
- **RC** : Release Candidate (pré-release)
- **Stable** : Version de production
- Pas de suffixe = Stable par défaut

---

**Une fois le repo créé, on pourra implémenter le système de mise à jour automatique dans Frameflow !** 🚀
