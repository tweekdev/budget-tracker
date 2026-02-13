# Budget Tracker 2026 — PWA

## Déployer sur GitHub Pages (gratuit)

### 1. Créer un repo GitHub
```bash
cd expense-tracker-pwa
git init
git add .
git commit -m "Budget Tracker PWA"
git branch -M main
git remote add origin https://github.com/TON_USERNAME/budget-tracker.git
git push -u origin main
```

### 2. Activer GitHub Pages
1. Va sur ton repo GitHub → **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: **main** / **(root)**
4. Clique **Save**
5. Attends 1-2 minutes, ton app sera sur `https://TON_USERNAME.github.io/budget-tracker/`

### 3. Installer sur iPhone
1. Ouvre l'URL dans **Safari** sur ton iPhone
2. Appuie sur le bouton **Partager** (carré avec flèche)
3. Choisis **Sur l'écran d'accueil**
4. Donne un nom → **Ajouter**
5. L'app apparaît sur ton écran d'accueil comme une vraie app !

## Fonctionnalités
- **Persistance** : Toutes les données sont sauvegardées dans localStorage
- **Charges fixes** : Loyer, crédits, abonnements — avec status payé/non payé
- **Charges variables** : Eau, gaz, etc. — avec status payé/non payé
- **Dépenses plaisir** : Courses, shopping, etc. — avec status prélevé/en attente
- **Épargne** : Soldes bancaires réels + objectifs
- **Stats** : Règle 50/30/20, tendances, budget vs réel
- **PWA** : Fonctionne hors-ligne, installable sur iPhone/Android
- **Bouton +** : Ajouter une dépense depuis n'importe quel écran

## Structure
```
expense-tracker-pwa/
├── index.html      ← App complète (React + Recharts)
├── manifest.json   ← Config PWA (icône, couleurs)
├── sw.js           ← Service Worker (cache offline)
└── README.md
```
