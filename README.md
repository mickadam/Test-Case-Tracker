# 🧪 Test Case Tracker

> **Outil de suivi en temps réel pour vos cas de test**

Une application web moderne et intuitive pour gérer, organiser et suivre vos cas de test avec une interface responsive et des fonctionnalités avancées d'export/import.

## ✨ Fonctionnalités Principales

### 🎯 Gestion des Jeux de Test
- **Création personnalisée** de nouveaux jeux de test
- **Filtrage global** par jeu de test
- **Statistiques en temps réel** par domaine

### 📝 Création de Cas de Test
- **Ajout d'étapes** avec validation par Entrée
- **Timer automatique** dès la première étape
- **Étapes sauvegardées** pour réutilisation rapide
- **Édition inline** des résultats et statuts

### 👀 Modes d'Affichage
- **Vue détaillée** : Cartes complètes avec toutes les informations
- **Vue en ligne** : Affichage condensé avec flux d'étapes
- **Regroupement automatique** par jeu de test

### 📊 Export et Analyse
- **Export CSV** pour analyse dans Excel/Google Sheets
- **Export Markdown** pour documentation
- **Export TXT** pour rapports simples
- **Import CSV** pour récupération de données

### 💾 Persistance
- **Sauvegarde automatique** dans le navigateur
- **Récupération** au rechargement de page
- **Données conservées** : Cas de test, étapes, jeux personnalisés

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
   - Définissez le résultat et le statut
   - Sauvegardez votre cas de test

## 📁 Structure du Projet

```
Test-Case-Tracker/
├── index.html             # Application principale
├── docs/
│   ├── SPECIFICATION.md    # Spécifications détaillées
│   └── AGENTS.md          # Architecture et agents
├── assets/                 # Ressources statiques
├── .github/
│   └── workflows/         # GitHub Actions pour déploiement automatique
├── 404.html               # Page d'erreur personnalisée
├── DEPLOYMENT.md          # Guide de déploiement GitHub Pages
├── README.md              # Ce fichier
└── LICENSE                # Licence MIT
```

## 🎮 Utilisation

### Création d'un Cas de Test
1. **Sélectionner un jeu de test** (ou en créer un nouveau)
2. **Ajouter des étapes** une par une
3. **Définir le résultat observé**
4. **Choisir le statut** (✅ OK / ❌ KO / ⏳ En cours)
5. **Sauvegarder** le cas de test

### Édition Rapide
- **Clic sur le statut** : Cycle automatique OK → KO → En cours
- **Clic sur le résultat** : Édition inline avec validation
- **Bouton 🗑️** : Suppression avec confirmation

### Export de Données
- **📄 Exporter les Résultats** : Choix du format (CSV, Markdown, TXT)
- **📊 Stats** : Statistiques par jeu de test
- **Import CSV** : Récupération de données sauvegardées

## 🛠️ Technologies

- **Frontend** : HTML5, CSS3, JavaScript ES6+ (vanilla)
- **Stockage** : localStorage (navigateur)
- **Design** : CSS Grid, Flexbox, Animations CSS
- **Architecture** : Agent-based pattern
- **Dépendances** : **Aucune !** 🎉 (HTML/CSS/JS pur)
- **Installation** : **Aucune !** 🚀 (Double-clic et c'est parti)

## 📋 Cas d'Usage

### Tests Exploratoires
- Prise de notes rapide pendant l'exploration
- Réutilisation d'étapes communes
- Correction immédiate des résultats

### Tests de Non-Régression
- Organisation par domaines fonctionnels
- Suivi des taux de succès
- Export pour documentation

### Tests Collaboratifs
- Étapes standardisées réutilisables
- Vision claire des résultats par domaine
- Partage facile avec les développeurs

## 🤝 Contribution

Les contributions sont les bienvenues ! Pour contribuer :

1. Fork le projet
2. Créer une branche feature (`git checkout -b feature/nouvelle-fonctionnalite`)
3. Commit vos changements (`git commit -am 'Ajout nouvelle fonctionnalité'`)
4. Push vers la branche (`git push origin feature/nouvelle-fonctionnalite`)
5. Ouvrir une Pull Request

## 📄 Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

## 🆘 Support

- **Documentation** : Consultez [docs/SPECIFICATION.md](docs/SPECIFICATION.md)
- **Architecture** : Voir [AGENTS.md](AGENTS.md)
- **Déploiement** : Guide complet dans [DEPLOYMENT.md](DEPLOYMENT.md)
- **Issues** : Utilisez les GitHub Issues pour signaler des bugs

---

**Développé avec ❤️ pour simplifier le suivi de vos cas de test !** 🚀
