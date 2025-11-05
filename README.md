# GradientGen - Guide d'hébergement gratuit

## 🚀 Options d'hébergement gratuites

Votre application est une application web statique qui peut être hébergée gratuitement sur plusieurs plateformes.

### Option 1 : GitHub Pages (Le plus simple !)

**Étapes :**

1. **Créer un compte GitHub** (si vous n'en avez pas) : https://github.com

2. **Créer un nouveau dépôt** :
   - Cliquez sur "New repository"
   - Nommez-le (ex: `gradientgen`)
   - Choisissez "Public"
   - Cliquez sur "Create repository"

3. **Uploader vos fichiers** :
   - Téléchargez GitHub Desktop : https://desktop.github.com
   - Ou utilisez les commandes suivantes dans votre terminal :

```bash
cd "C:\Users\noega\Desktop\FreeTool1"
git init
git add .
git commit -m "Première version"
git branch -M main
git remote add origin https://github.com/VOTRE-NOM/gradientgen.git
git push -u origin main
```

4. **Activer GitHub Pages** :
   - Allez dans votre dépôt sur GitHub
   - Cliquez sur "Settings" (Paramètres)
   - Dans le menu de gauche, cliquez sur "Pages"
   - Sous "Source", sélectionnez "main" (ou "master")
   - Cliquez sur "Save"
   - Votre site sera disponible à : `https://VOTRE-NOM.github.io/gradientgen`

### Option 2 : Netlify (Très simple avec drag & drop !)

**Étapes :**

1. **Aller sur Netlify** : https://www.netlify.com
2. **Créer un compte gratuit** (avec GitHub, Google, ou email)
3. **Glisser-déposer votre dossier** `FreeTool1` sur la page Netlify
4. **C'est tout !** Vous obtenez une URL immédiatement

**Avantages :**
- URL personnalisée (ex: `votre-nom.netlify.app`)
- Déploiement automatique si vous utilisez Git
- HTTPS gratuit
- Très rapide

### Option 3 : Vercel (Excellente performance)

**Étapes :**

1. **Aller sur Vercel** : https://vercel.com
2. **Créer un compte gratuit**
3. **Importer votre projet** (via GitHub ou drag & drop)
4. **Déployer !**

### Option 4 : Cloudflare Pages

**Étapes :**

1. **Aller sur Cloudflare Pages** : https://pages.cloudflare.com
2. **Créer un compte gratuit**
3. **Connecter votre dépôt GitHub** ou uploader manuellement
4. **Déployer !**

## 📁 Structure des fichiers

Votre application contient :
- `index.html` - Page principale
- `sketch.js` - Code JavaScript (contient maintenant le shader intégré)
- `styles.css` - Styles CSS
- `Image.frag` - Shader WebGL (optionnel, maintenant intégré dans sketch.js)
- `BergenMono-Regular.otf` - Police de caractères

**Note importante :** Le shader `Image.frag` est maintenant intégré directement dans `sketch.js` pour éviter les problèmes CORS lors de l'ouverture en local (file://). L'application fonctionne maintenant même si vous ouvrez simplement le fichier HTML dans votre navigateur sans serveur web !

Tous ces fichiers doivent être dans le même dossier à la racine.

## ⚡ Mise à jour

Pour mettre à jour votre site :

**GitHub Pages :**
- Modifiez vos fichiers localement
- Committez et poussez sur GitHub
- Le site se met à jour automatiquement en quelques minutes

**Netlify/Vercel :**
- Si connecté à GitHub : push automatique
- Sinon : re-glissez votre dossier mis à jour

## 🌐 Partagez votre URL

Une fois déployé, vous pouvez partager l'URL avec n'importe qui !

## 💡 Conseil

Pour un nom de domaine personnalisé (optionnel, gratuit sur certains services) :
- Netlify et Vercel permettent d'ajouter un domaine personnalisé gratuitement
- Vous pouvez aussi utiliser un sous-domaine gratuit sur Freenom
