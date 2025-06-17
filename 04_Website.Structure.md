# 🌐 Architecture d'un Site Web - Structure Simple

Guide rapide pour organiser les dossiers et fichiers de votre site web.

---

## 📁 Structure de Base

```
mon-site/
├── index.html              # Page d'accueil (obligatoire)
├── about.html              # Page à propos
├── contact.html            # Page contact
├── css/                    # Styles CSS
│   ├── style.css          # CSS principal
│   └── responsive.css     # CSS mobile
├── js/                     # Scripts JavaScript
│   ├── main.js            # JS principal
│   └── components.js      # JS des composants
├── images/                 # Images et médias
│   ├── logo.png
│   ├── banner.jpg
│   └── gallery/
│       ├── photo1.jpg
│       └── photo2.jpg
└── fonts/                  # Polices (optionnel)
    └── custom-font.woff
```

---

## 🏗️ Structure Avancée

Pour un site plus complexe :

```
mon-site/
├── index.html
├── pages/                  # Pages secondaires
│   ├── services.html
│   ├── portfolio.html
│   └── blog/
│       ├── index.html
│       ├── article-1.html
│       └── article-2.html
├── assets/                 # Ressources
│   ├── css/
│   │   ├── main.css
│   │   ├── components.css
│   │   └── utilities.css
│   ├── js/
│   │   ├── app.js
│   │   ├── modules/
│   │   │   ├── slider.js
│   │   │   └── modal.js
│   │   └── vendor/         # Librairies externes
│   │       └── jquery.min.js
│   ├── images/
│   │   ├── ui/             # Images interface
│   │   ├── content/        # Images contenu
│   │   └── icons/          # Icônes
│   └── fonts/
├── docs/                   # Documentation
│   ├── README.md          # Documentation projet
│   └── CHANGELOG.md       # Historique des versions
├── .gitignore             # Fichiers à ignorer par Git
├── .gitattributes         # Configuration Git
├── README.md              # Description du projet
└── LICENSE                # Licence du projet
```

---

## 📋 Règles de Nommage

### ✅ Bonnes pratiques

- **Minuscules uniquement** : `style.css`, `main.js`
- **Tirets pour séparer** : `hero-banner.jpg`, `contact-form.html`
- **Noms descriptifs** : `navigation.css`, `slider.js`
- **Pas d'espaces** : `mon-projet.html` (pas `mon projet.html`)

### ❌ À éviter

- Caractères spéciaux : `style&design.css`
- Espaces : `mon script.js`
- Majuscules : `STYLE.CSS`
- Noms génériques : `image1.jpg`, `page2.html`

---

## 🎯 Types de Fichiers

### HTML

- **index.html** : Page d'accueil (toujours à la racine)
- **Pages principales** : `about.html`, `contact.html`, `services.html`
- **Sous-pages** : Dans le dossier `pages/`

### CSS

- **main.css** : Styles principaux
- **responsive.css** : Styles mobile/tablette
- **components.css** : Styles des composants réutilisables

### JavaScript

- **main.js** : Script principal
- **components.js** : Scripts des composants
- **vendor/** : Librairies externes (jQuery, Bootstrap...)

### Images

- **Formats recommandés** : `.jpg`, `.png`, `.svg`, `.webp`
- **Organisation** : Par type ou par page
- **Optimisation** : Compresser avant upload

---

## 🔗 Chemins et Liens

### Liens relatifs

```html
<!-- Depuis index.html -->
<link rel="stylesheet" href="css/style.css" />
<img src="images/logo.png" alt="Logo" />
<a href="about.html">À propos</a>

<!-- Depuis une sous-page -->
<link rel="stylesheet" href="../css/style.css" />
<img src="../images/logo.png" alt="Logo" />
<a href="../index.html">Accueil</a>
```

### Organisation logique

- **CSS** : Toujours dans `<head>`
- **JS** : Avant la fermeture `</body>`
- **Images** : Avec attribut `alt` obligatoire

---

## 📱 Structure Responsive

### Breakpoints CSS

```css
/* Mobile first */
@media (min-width: 768px) {
  /* Tablette */
}
@media (min-width: 1024px) {
  /* Desktop */
}
```

### Organisation mobile

- **Menu burger** : Pour petits écrans
- **Grilles flexibles** : CSS Grid ou Flexbox
- **Images adaptatives** : `max-width: 100%`

---

## ⚡ Optimisation

### Performance

- **Minifier** CSS et JS en production
- **Optimiser** les images (compression)
- **Lazy loading** pour les images
- **Cache** navigateur avec headers appropriés

### SEO

- **Balises meta** dans chaque page
- **Structure sémantique** HTML5
- **URLs propres** : `contact.html` plutôt que `page2.html`
- **Sitemap.xml** pour gros sites

---

## 🛠️ Outils Recommandés

### Éditeurs

- **VS Code** avec extensions
- **Sublime Text**
- **WebStorm**

### Validation

- **HTML Validator** (W3C)
- **CSS Validator** (W3C)
- **Lighthouse** (performance)

### Déploiement

- **GitHub Pages** (gratuit)
- **Netlify** (gratuit)
- **FTP** traditionnel

---

## 📄 Fichiers de Configuration

### .gitignore

Fichier pour ignorer certains éléments lors du versioning :

```
# Fichiers système
.DS_Store
Thumbs.db
desktop.ini

# Éditeurs
.vscode/
.idea/
*.swp
*.swo

# Dossiers temporaires
node_modules/
.cache/
dist/
build/

# Fichiers de log
*.log
npm-debug.log*

# Fichiers de sauvegarde
*.bak
*.tmp
*~

# Fichiers sensibles
.env
config.local.js
```

### README.md

Documentation du projet :

```markdown
# Mon Site Web

Description courte du projet.

## Installation

1. Cloner le repository
2. Ouvrir index.html dans un navigateur

## Structure

- `css/` : Feuilles de style
- `js/` : Scripts JavaScript
- `images/` : Médias et images

## Auteur

Votre nom - contact@email.com
```

### LICENSE

Licence du projet (MIT, GPL, etc.) selon vos besoins.

---

## 🔧 Configuration Git

### Initialisation

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin [URL-DU-REPO]
git push -u origin main
```

### Commits recommandés

```bash
git commit -m "feat: add contact page"
git commit -m "fix: correct navigation menu"
git commit -m "style: update CSS responsive"
git commit -m "docs: update README"
```

---

## 📝 Checklist Finale

Avant de mettre en ligne :

- [ ] `index.html` à la racine
- [ ] Tous les liens fonctionnent
- [ ] Images optimisées et avec `alt`
- [ ] CSS et JS bien liés
- [ ] Site testé sur mobile
- [ ] Validation HTML/CSS
- [ ] Favicon ajouté
- [ ] Meta descriptions renseignées
- [ ] `.gitignore` configuré
- [ ] `README.md` rédigé
- [ ] Repository Git initialisé
- [ ] Premier commit effectué
