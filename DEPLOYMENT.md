# 🚀 Guide de Déploiement GitHub Pages

## Configuration GitHub Pages

### 1. Activation de GitHub Pages

1. **Aller dans les paramètres du repository**
   - Cliquer sur `Settings` dans votre repository GitHub
   - Scroller jusqu'à la section `Pages`

2. **Configurer la source**
   - **Source** : `Deploy from a branch`
   - **Branch** : `main` (ou `gh-pages` si vous utilisez le workflow)
   - **Folder** : `/ (root)` - Le fichier `index.html` est à la racine

3. **Sauvegarder**
   - Cliquer sur `Save`
   - Votre site sera disponible à : `https://votre-username.github.io/Test-Case-Tracker/`

### 2. Workflow GitHub Actions

Le projet inclut un workflow automatique :

#### Workflow Principal (`pages.yml`)
- **Déclencheur** : Push sur la branche `main`
- **Action** : Déploiement automatique vers GitHub Pages
- **Permissions** : Configurées automatiquement
- **Méthode** : Moderne et recommandée par GitHub

### 3. Structure des Fichiers

```
Test-Case-Tracker/
├── index.html             # Application principale
├── .github/
│   └── workflows/         # Workflows GitHub Actions
├── docs/                  # Documentation
├── assets/                # Ressources statiques
└── README.md              # Documentation utilisateur
```

## Déploiement Manuel

### Option 1 : Déploiement Direct (Recommandé)
```bash
# Cloner le repository
git clone https://github.com/votre-username/Test-Case-Tracker.git
cd Test-Case-Tracker

# Pousser vers GitHub
git add .
git commit -m "Deploy to GitHub Pages"
git push origin main
```

### Option 2 : Déploiement via Branche gh-pages
```bash
# Créer et basculer sur la branche gh-pages
git checkout -b gh-pages

# Pousser la branche
git push origin gh-pages

# Configurer GitHub Pages pour utiliser gh-pages
```

**Note** : Aucune installation de dépendances requise ! L'application est 100% autonome.

## Vérification du Déploiement

### 1. Vérifier le Statut
- Aller dans l'onglet `Actions` de votre repository
- Vérifier que les workflows se sont exécutés avec succès
- Cliquer sur le workflow pour voir les détails

### 2. Tester le Site
- Visiter `https://votre-username.github.io/Test-Case-Tracker/`
- Vérifier que l'application se charge correctement
- Tester les fonctionnalités principales

### 3. Vérifier la Page 404
- Visiter une URL inexistante : `https://votre-username.github.io/Test-Case-Tracker/page-inexistante`
- Vérifier que la page 404 personnalisée s'affiche

## Configuration Avancée

### Variables d'Environnement
Aucune variable d'environnement nécessaire ! L'application est 100% côté client.

### Domaine Personnalisé
Pour utiliser un domaine personnalisé :
1. Ajouter un fichier `CNAME` à la racine
2. Configurer le DNS de votre domaine
3. Activer HTTPS dans les paramètres GitHub Pages

### Optimisations

#### Cache et Performance
- Les fichiers statiques sont automatiquement mis en cache
- GitHub Pages utilise un CDN global
- Compression automatique des assets

#### SEO
- Meta tags optimisés dans `index.html`
- Sitemap automatique (si nécessaire)
- Page 404 personnalisée pour une meilleure UX

## Dépannage

### Problèmes Courants

#### 1. Site ne se charge pas
- Vérifier que GitHub Pages est activé
- Vérifier la branche source dans les paramètres
- Attendre quelques minutes pour la propagation

#### 2. Erreur 404 sur toutes les pages
- Vérifier que `index.html` est à la racine
- Vérifier la configuration de la branche source

#### 3. Workflow en échec
- Vérifier les permissions du repository
- Vérifier la syntaxe des workflows
- Consulter les logs dans l'onglet Actions

### Logs et Debug
- **Actions** : Onglet Actions pour les logs de déploiement
- **Pages** : Section Pages dans Settings pour le statut
- **Network** : Outils développeur pour vérifier les requêtes

## Maintenance

### Mises à Jour
- Les mises à jour sont automatiques via les workflows
- Chaque push sur `main` déclenche un nouveau déploiement
- Aucune intervention manuelle nécessaire
- **Aucune dépendance à mettre à jour !**

### Sauvegarde
- Le code source est sauvegardé sur GitHub
- Les données utilisateur sont stockées dans localStorage
- Pas de base de données externe à sauvegarder
- **Application 100% autonome !**

---

**Votre Test Case Tracker est maintenant prêt pour GitHub Pages ! 🎉**
