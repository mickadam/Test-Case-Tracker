# 🧪 Test Case Tracker

> **Outil de suivi en temps réel pour vos cas de test avec capture d'écran et export avancé**

Une application web moderne et intuitive pour gérer, organiser et suivre vos cas de test avec une interface responsive, capture d'écran intégrée, et des fonctionnalités avancées d'export/import JSON.

## 🌐 Application en Ligne

**🚀 [Tester l'application directement](https://mickadam.github.io/Test-Case-Tracker/)**

L'application est déployée sur GitHub Pages et accessible immédiatement sans installation !

## ✨ Fonctionnalités Principales

### 🎯 Gestion des Jeux de Test
- **Création personnalisée** de nouveaux jeux de test
- **Filtrage global** par jeu de test
- **Statistiques en temps réel** par domaine
- **Mémorisation** du dernier jeu utilisé pour les nouveaux cas

### 📝 Création de Cas de Test
- **Ajout d'étapes** avec validation par Entrée
- **Timer automatique** dès la première étape
- **Étapes sauvegardées** pour réutilisation rapide
- **Édition inline** des résultats et statuts
- **Capture d'écran** intégrée pour chaque étape
- **Collage direct** depuis le presse-papier (Ctrl+V)

### 📷 Gestion des Images
- **Upload d'images** depuis l'ordinateur
- **Collage de screenshots** depuis le presse-papier
- **Miniatures** avec aperçu au survol
- **Modal plein écran** pour visualisation détaillée
- **Stockage optimisé** en Base64 dans le navigateur

### 👀 Modes d'Affichage
- **Vue détaillée** : Cartes complètes avec toutes les informations
- **Vue en ligne** : Affichage condensé avec flux d'étapes
- **Regroupement automatique** par jeu de test
- **Indicateurs visuels** pour les étapes avec images

### 📊 Export et Analyse Avancés
- **Export JSON** : Sauvegarde complète avec images
- **Export ZIP** : Archive avec CSV, Markdown et images
- **Export Markdown** : Documentation avec liens d'images
- **Export TXT** : Rapport simple avec indicateurs d'images
- **Import JSON** : Restauration complète sans perte de données
- **Filtrage par jeu** : Export uniquement du jeu sélectionné

### 💾 Persistance Intelligente
- **Sauvegarde automatique** dans le navigateur
- **Récupération** au rechargement de page
- **Données conservées** : Cas de test, étapes, jeux, images
- **Mémorisation** du dernier jeu de test utilisé
- **Import intelligent** : Ajout sans doublons

## 🚀 Démarrage Rapide

1. **Cloner le projet**
   ```bash
   git clone https://github.com/votre-username/Test-Case-Tracker.git
   cd Test-Case-Tracker
   ```

2. **Ouvrir l'application**
   
   **Option 1: Directement dans le navigateur (le plus simple)**
   - Double-cliquer sur `index.html`
   - Ou faire clic-droit → "Ouvrir avec" → votre navigateur
   - ✅ **Aucune installation requise !**
   
   **Option 2: Serveur local (optionnel)**
   ```bash
   # Si vous avez Python installé :
   python -m http.server 8000
   # Puis aller sur http://localhost:8000/
   
   # Ou avec Node.js :
   npx serve .
   ```
   
   **Option 3: GitHub Pages (pour partage/publication)**
   - Voir [DEPLOYMENT.md](DEPLOYMENT.md) pour la configuration
   - ✅ **Aucune installation requise côté utilisateur !**

3. **Commencer à tester**
   - Sélectionnez ou créez un jeu de test
   - Ajoutez vos étapes de test
   - Ajoutez des screenshots si nécessaire
   - Définissez le résultat et le statut
   - Sauvegardez votre cas de test

## 📁 Structure du Projet

```
Test-Case-Tracker/
├── index.html             # Application principale (monolithe)
├── docs/
│   └── SPECIFICATION.md    # Spécifications détaillées
├── .github/
│   └── workflows/         # GitHub Actions pour déploiement automatique
│       └── pages.yml      # Workflow de déploiement GitHub Pages
├── AGENTS.md              # Architecture et agents
├── DEPLOYMENT.md          # Guide de déploiement GitHub Pages
├── README.md              # Ce fichier
└── LICENSE                # Licence CC0-1.0
```

## 🎮 Utilisation

### Création d'un Cas de Test
1. **Sélectionner un jeu de test** (ou en créer un nouveau)
2. **Ajouter des étapes** une par une
3. **Ajouter des screenshots** (optionnel) :
   - 📷 Charger depuis l'ordinateur
   - 📋 Coller depuis le presse-papier (Ctrl+V)
4. **Définir le résultat observé**
5. **Choisir le statut** (✅ OK / ❌ KO / ⏳ En cours)
6. **Sauvegarder** le cas de test

### Édition Rapide
- **Clic sur le statut** : Cycle automatique OK → KO → En cours
- **Clic sur le résultat** : Édition inline multi-ligne
- **Clic sur les étapes** : Édition inline des étapes
- **Bouton 🗑️** : Suppression avec confirmation

### Export de Données
- **📄 Export JSON** : Sauvegarde complète avec images
- **📦 Export ZIP** : Archive avec CSV, Markdown et images
- **📝 Export Markdown** : Documentation avec liens d'images
- **📄 Export TXT** : Rapport simple
- **📥 Import JSON** : Restauration complète

### Gestion des Images
- **Aperçu** : Miniature au survol de l'indicateur 📷
- **Visualisation** : Clic pour ouvrir en modal plein écran
- **Export** : Images incluses dans les exports ZIP et Markdown

## 🛠️ Technologies

- **Frontend** : HTML5, CSS3, JavaScript ES6+ (vanilla)
- **Stockage** : localStorage (navigateur)
- **Images** : Base64 encoding, Canvas API
- **Clipboard** : Clipboard API pour le collage
- **Archives** : JSZip pour les exports ZIP
- **Design** : CSS Grid, Flexbox, Animations CSS
- **Architecture** : Agent-based pattern
- **Dépendances** : **Aucune !** 🎉 (HTML/CSS/JS pur)
- **Installation** : **Aucune !** 🚀 (Double-clic et c'est parti)

## 📋 Cas d'Usage

### Tests Exploratoires
- Prise de notes rapide pendant l'exploration
- Capture d'écran des anomalies
- Réutilisation d'étapes communes
- Correction immédiate des résultats

### Tests de Non-Régression
- Organisation par domaines fonctionnels
- Screenshots des résultats attendus
- Suivi des taux de succès
- Export pour documentation

### Tests Collaboratifs
- Étapes standardisées réutilisables
- Screenshots partagés avec l'équipe
- Vision claire des résultats par domaine
- Partage facile avec les développeurs

### Tests d'Interface
- Capture d'écran des états de l'interface
- Documentation visuelle des bugs
- Comparaison avant/après
- Rapport visuel complet

## 🔄 Workflow d'Export/Import

### Export Complet
1. **Sélectionner un jeu de test** (optionnel)
2. **Cliquer "📄 Exporter les Résultats"**
3. **Choisir "📄 Export JSON"**
4. **Fichier téléchargé** avec toutes les données

### Import Intelligent
1. **Cliquer "📥 Importer JSON"**
2. **Sélectionner le fichier JSON**
3. **Confirmer l'import**
4. **Données ajoutées** sans doublons

### Sauvegarde/Partage
- **Export JSON** : Sauvegarde complète
- **Export ZIP** : Partage avec images
- **Import JSON** : Restauration fidèle

## 🤝 Contribution

Les contributions sont les bienvenues ! Pour contribuer :

1. Fork le projet
2. Créer une branche feature (`git checkout -b feature/nouvelle-fonctionnalite`)
3. Commit vos changements (`git commit -am 'Ajout nouvelle fonctionnalité'`)
4. Push vers la branche (`git push origin feature/nouvelle-fonctionnalite`)
5. Ouvrir une Pull Request

## 📄 Licence

Ce projet est sous licence CC0-1.0. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

## 🆘 Support

- **Documentation** : Consultez [docs/SPECIFICATION.md](docs/SPECIFICATION.md)
- **Architecture** : Voir [AGENTS.md](AGENTS.md)
- **Déploiement** : Guide complet dans [DEPLOYMENT.md](DEPLOYMENT.md)
- **Issues** : Utilisez les GitHub Issues pour signaler des bugs

## 🆕 Nouvelles Fonctionnalités

### Version Actuelle
- ✅ **Capture d'écran intégrée** pour chaque étape
- ✅ **Collage depuis le presse-papier** (Ctrl+V)
- ✅ **Export JSON complet** avec images
- ✅ **Import intelligent** sans doublons
- ✅ **Export ZIP** avec CSV, Markdown et images
- ✅ **Mémorisation** du dernier jeu de test utilisé
- ✅ **Édition multi-ligne** des résultats
- ✅ **Aperçu d'images** au survol

---

**Développé avec ❤️ pour simplifier le suivi de vos cas de test avec capture d'écran !** 🚀📷