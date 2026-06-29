# SILOE-BUY A.P — Pages de Vente

## Structure du projet

```
siloebuy-pages/
├── public/
│   ├── index.html          ← Page d'accueil (hub des 2 produits)
│   ├── import-chine.html   ← Page de vente Import Chine Sans Arnaque
│   └── formation-excel.html← Page de vente Formation Excel & VBA
├── vercel.json             ← Configuration Vercel
└── README.md
```

## URLs après déploiement

| Page | URL |
|------|-----|
| Accueil | `https://votre-projet.vercel.app/` |
| Import Chine | `https://votre-projet.vercel.app/import-chine` |
| Formation Excel | `https://votre-projet.vercel.app/formation-excel` |

## Pixel Meta

Le Pixel ID **754178417315236** est intégré dans les 3 pages avec :
- `PageView` automatique sur chaque page
- `ViewContent` sur clic vers chaque formation (depuis l'accueil)

## Déploiement — 3 méthodes

### Méthode 1 : Vercel CLI (recommandé)

```bash
npm install -g vercel
cd siloebuy-pages
vercel
# Suivre les instructions → projet créé automatiquement
```

### Méthode 2 : Interface web Vercel (le plus simple)

1. Aller sur **vercel.com** → Se connecter
2. Cliquer **"Add New → Project"**
3. Glisser-déposer le dossier `siloebuy-pages` OU importer depuis GitHub
4. Vercel détecte automatiquement `outputDirectory: "public"`
5. Cliquer **Deploy** ✓

### Méthode 3 : Via GitHub

1. Créer un repo GitHub `siloebuy-pages`
2. Push les fichiers
3. Sur Vercel → Import depuis GitHub
4. Auto-déploiement à chaque push

## Domaine personnalisé

Après déploiement, dans le dashboard Vercel :
- Settings → Domains → Ajouter `pages.siloebuy.com` ou votre domaine

## Liens de paiement Chariow

- Import Chine : `https://siloebuy.mychariow.shop/prd_edjnu9kx/checkout`
- Formation Excel : `https://siloebuy.mychariow.shop/prd_7ryxae/checkout`

## Taille des fichiers

| Fichier | Taille |
|---------|--------|
| index.html | ~15 KB |
| import-chine.html | ~916 KB (bundle autonome) |
| formation-excel.html | ~1.73 MB (bundle autonome) |
