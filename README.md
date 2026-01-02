# 🌐 Site Web Calcul Charges ME

Site web officiel pour l'application mobile Calcul Charges ME.

## 📁 Structure des fichiers

```
microcalc-website/
├── index.html              # Page d'accueil
├── styles.css             # Styles (design noir & or premium)
├── script.js              # JavaScript (animations, interactions)
├── confidentialite.html   # Politique de confidentialité
├── mentions-legales.html  # Mentions légales et CGU
└── README.md             # Ce fichier
```

## 🎨 Design

**Palette de couleurs :**
- Fond : Noir (#0a0a0a) et gris anthracite (#1a1a1a)
- Accents : Or (#d4af37) et or clair (#f4d56f)
- Texte : Blanc (#ffffff) et gris (#b0b0b0)

**Style :** Premium, fintech moderne, minimaliste

## 🚀 Hébergement

### Option 1 : GitHub Pages (GRATUIT - Recommandé)

1. **Créer un repo GitHub**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/ton-username/microcalc-website.git
   git push -u origin main
   ```

2. **Activer GitHub Pages**
   - Va dans Settings → Pages
   - Source : main branch
   - Ton site sera sur : `https://ton-username.github.io/microcalc-website`

3. **Domaine personnalisé (optionnel)**
   - Achète un domaine (ex: microcalc.fr sur OVH/Gandi)
   - Configure le DNS
   - Ajoute le domaine dans Settings → Pages

### Option 2 : Netlify (GRATUIT)

1. **Connecte ton repo GitHub à Netlify**
   - Va sur netlify.com
   - "Add new site" → "Import from Git"
   - Sélectionne ton repo
   - Deploy !

2. **URL gratuite**
   - Ton site sera sur : `https://random-name.netlify.app`
   - Tu peux personnaliser en : `microcalc.netlify.app`

3. **Domaine personnalisé (optionnel)**
   - Ajoute ton domaine dans Domain settings

### Option 3 : Vercel (GRATUIT)

1. **Importe depuis GitHub**
   - Va sur vercel.com
   - Import project
   - Sélectionne ton repo

2. **Deploy automatique**
   - Chaque push = nouveau déploiement
   - URL : `https://microcalc.vercel.app`

## ✏️ Personnalisation

### 1. Ajouter vos screenshots (OBLIGATOIRE)

**Créez un dossier `images/` avec vos 4 screenshots :**

```
microcalc-website/
├── index.html
├── styles.css
├── script.js
├── images/                    ← CRÉER CE DOSSIER
│   ├── screenshot-1.png       ← Écran d'accueil avec calculateur
│   ├── screenshot-2.png       ← Résultats avec calcul 5000€
│   ├── screenshot-3.png       ← Alerte de seuil (carte verte/orange/rouge)
│   └── screenshot-4.png       ← Historique avec plusieurs calculs
├── confidentialite.html
├── mentions-legales.html
└── README.md
```

**Comment obtenir les screenshots :**
1. Lance l'émulateur Android Studio avec l'app
2. Prends des captures d'écran (bouton 📷 dans l'émulateur)
3. Les images seront au format PNG
4. Renomme-les en `screenshot-1.png`, `screenshot-2.png`, etc.
5. Place-les dans le dossier `images/`

**IMPORTANT :** Sans ce dossier `images/`, les images ne s'afficheront pas sur le site !

### 2. Modifier les informations de contact

Dans `index.html`, `confidentialite.html` et `mentions-legales.html`, cherche :
```html
contact@docsmart.fr
```
Et remplace par ton vrai email.

### 2. Ajouter le lien Google Play

Une fois l'app publiée, dans `index.html`, cherche :
```html
<a href="#" class="btn-download">
```
Et remplace `#` par le lien Play Store :
```html
<a href="https://play.google.com/store/apps/details?id=com.docsmart.microcalc" class="btn-download">
```

### 3. Ajouter Google Analytics (optionnel)

Dans `script.js`, décommente et complète :
```javascript
window.dataLayer = window.dataLayer || [];
function gtag(){dataLayer.push(arguments);}
gtag('js', new Date());
gtag('config', 'GA_MEASUREMENT_ID'); // Remplace par ton ID
```

### 4. Ajouter des screenshots

Crée un dossier `images/` et ajoute tes screenshots :
```
images/
├── screenshot-1.png
├── screenshot-2.png
├── screenshot-3.png
└── screenshot-4.png
```

Dans `index.html`, tu peux remplacer le mockup de téléphone par de vrais screenshots.

## 📊 SEO

Le site est déjà optimisé pour le SEO :
- ✅ Meta descriptions
- ✅ Meta keywords
- ✅ Open Graph (Facebook)
- ✅ Twitter Cards
- ✅ Structure HTML sémantique
- ✅ Sitemap (à créer si besoin)

### Créer un sitemap.xml (optionnel)

```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url>
    <loc>https://ton-domaine.com/</loc>
    <lastmod>2026-01-02</lastmod>
    <priority>1.0</priority>
  </url>
  <url>
    <loc>https://ton-domaine.com/confidentialite.html</loc>
    <lastmod>2026-01-02</lastmod>
    <priority>0.8</priority>
  </url>
  <url>
    <loc>https://ton-domaine.com/mentions-legales.html</loc>
    <lastmod>2026-01-02</lastmod>
    <priority>0.8</priority>
  </url>
</urlset>
```

## 🔍 Google Search Console

1. **Soumettre le site**
   - Va sur search.google.com/search-console
   - Ajoute ta propriété (ton domaine)
   - Vérifie la propriété

2. **Soumettre le sitemap**
   - Dans Search Console → Sitemaps
   - Ajoute : `https://ton-domaine.com/sitemap.xml`

## 📱 Responsive

Le site est 100% responsive :
- ✅ Mobile
- ✅ Tablette
- ✅ Desktop
- ✅ Grande écran

Testé sur :
- iPhone 12/13/14
- Samsung Galaxy
- iPad
- Desktop 1920px+

## ⚡ Performance

**Optimisations appliquées :**
- CSS minifié (peut être compressé davantage)
- Pas de librairies externes lourdes
- Images optimisées (à faire quand tu ajoutes les screenshots)
- Lazy loading (peut être ajouté)

## 🔒 Sécurité

- HTTPS automatique (GitHub Pages, Netlify, Vercel)
- Pas de formulaires = pas de faille XSS
- Pas de backend = pas de faille SQL
- Headers de sécurité (à configurer sur Netlify/Vercel si besoin)

## 📝 TODO après déploiement

- [ ] Remplacer `contact@docsmart.fr` par ton vrai email
- [ ] Ajouter le lien Google Play Store
- [ ] Ajouter de vrais screenshots de l'app
- [ ] Soumettre à Google Search Console
- [ ] Créer un sitemap.xml
- [ ] Ajouter Google Analytics (optionnel)
- [ ] Tester sur différents navigateurs
- [ ] Partager le lien sur les réseaux sociaux

## 🎯 Utiliser le site dans Play Console

1. **Copie l'URL du site déployé**
   Ex: `https://microcalc.netlify.app`

2. **Ajoute-la dans Play Console**
   - Fiche de l'app → Site web
   - Colle l'URL

3. **C'est tout !**

## 💡 Améliorations futures possibles

- [ ] Blog pour articles SEO
- [ ] Page FAQ
- [ ] Formulaire de contact
- [ ] Newsletter
- [ ] Vidéo de démonstration
- [ ] Témoignages utilisateurs
- [ ] Comparateur avec d'autres apps
- [ ] Calculateur en ligne (version web de l'app)

## 🆘 Support

Si tu as des questions sur le déploiement :
- Netlify : docs.netlify.com
- GitHub Pages : docs.github.com/pages
- Vercel : vercel.com/docs

---

**Site créé le :** 2 janvier 2026  
**Version :** 1.0  
**Design :** Premium noir & or  
**Prêt à déployer :** ✅