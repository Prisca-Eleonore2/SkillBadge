# 🎓 SkillBadge - Site Vitrine

Bienvenue sur le site vitrine officiel de **SkillBadge** – le système de certification numérique basé sur la blockchain pour valoriser les compétences des jeunes autodidactes au Burkina Faso et en Afrique.

## 📋 Structure du Projet

```
Site Vitrine Sillbadge/
├── index.html       # Fichier principal HTML
├── styles.css       # Feuille de styles CSS
├── script.js        # Interactions JavaScript
├── README.md        # Ce fichier
└── assets/          # Dossier pour images et ressources (à créer au besoin)
```

## 🚀 Démarrage Rapide

### Option 1: Ouvrir directement dans un navigateur
1. Double-cliquez sur `index.html`
2. Le site s'ouvrira dans votre navigateur par défaut

### Option 2: Avec un serveur local (recommandé)
Si vous avez Python d'installé:
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```
Puis ouvrez `http://localhost:8000` dans votre navigateur.

Avec Node.js (si vous avez VS Code et Live Server):
- Installez l'extension "Live Server" dans VS Code
- Clic droit sur `index.html` → "Open with Live Server"

## 📱 Sections du Site

### 1. **Navigation** (Navbar)
- Collante en haut
- Responsive (menu hamburger sur mobile)
- Liens vers toutes les sections

### 2. **Hero Section** (Accueil)
- Titre principal et sous-titre
- Call-to-action (CTA) boutons
- Animation badge flottant
- Gradient moderne

### 3. **Présentation du Projet**
- Description SkillBadge
- 4 features principales avec icônes
- Visualisation Problème → Solution

### 4. **À Propos**
- Vision et mission du projet
- Liste des valeurs
- Présentation de l'équipe (4 rôles)

### 5. **FAQ**
- 6 questions fréquentes
- Accordéon interactif (clic pour ouvrir/fermer)
- Réponses complètes sur les badges

### 6. **Actualités & Blog**
- 3 articles d'exemple avec images
- Gradient background pour chaque article
- "Lire la suite" avec animation

### 7. **Contact**
- Informations de contact (email, téléphone, adresse, réseaux)
- Formulaire de contact fonctionnel
- Validation simple avec JavaScript

### 8. **Footer**
- Navigation rapide
- Liens légaux
- Crédits SkillBadge

## 🎨 Personnalisation

### Modifier les Couleurs
Cherchez dans `styles.css`:
```css
/* Couleur principale actuelle: Violet/Bleu */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);

/* Remplacez par vos couleurs */
/* Exemple nuances de vert
#2ecc71 (vert émeraude)
#27ae60 (vert foncé)
*/
```

### Modifier le Texte et le Contenu
Tous les textes sont dans `index.html`. Recherchez et remplacez:
- Titres et sous-titres
- Descriptions
- Noms de l'équipe
- Questions FAQ

### Ajouter des Images
1. Créez un dossier `assets/images/`
2. Placez vos images dedans
3. Dans `index.html`, remplacez les placeholders:

```html
<!-- De -->
<div class="blog-image" style="background: linear-gradient(...)"></div>

<!-- À -->
<div class="blog-image" style="background-image: url('assets/images/votre-image.jpg'); background-size: cover;"></div>
```

### Modifier les Informations de Contact
Dans la section contact, mettez à jour:
```html
<p>contact@skillbadge.bf</p>
<p>+226 XX XX XX XX</p>
<p>Ouagadougou, Burkina Faso</p>
```

## 🔧 Fonctionnalités JavaScript

### FAQ Interactive
- Clic sur une question pour l'ouvrir/fermer
- Une seule FAQ ouverte à la fois
- Animation avec icône rotative

### Formulaire de Contact
- Validation basique des champs
- Alert de confirmation
- Prêt pour intégration backend

### Menu Responsive
- Hamburger menu sur mobile
- Se ferme en cliquant un lien
- Se ferme en cliquant ailleurs

### Animations
- Apparition progressive au scroll
- Badges qui flottent
- Transitions lisses

### Dark Mode Support (optionnel)
Pour ajouter le dark mode, modifiez les styles dans `styles.css`:

```css
@media (prefers-color-scheme: dark) {
    body {
        background: #1a1a1a;
        color: #fff;
    }
    /* Ajustez tous les éléments */
}
```

## 📊 SEO & Métadonnées

Les balises meta essentielles sont présentes:
- `charset` UTF-8
- `viewport` responsive
- `description` pour les moteurs de recherche
- `title` optimisé

Pour améliorer le SEO:
1. Ajoutez des balises `<meta name="keywords">`
2. Structurez avec des balises sémantiques (`<article>`, `<section>`)
3. Optimisez les images avec `alt` text
4. Vérifiez dans Google Search Console

## 🌐 Déploiement

### Option 1: GitHub Pages (Gratuit)
1. Créez un repo GitHub nommé `skillbadge-vitrine`
2. Poussez tous les fichiers
3. Allez dans Settings → Pages
4. Sélectionnez "main" comme source
5. Votre site sera à `https://yourusername.github.io/skillbadge-vitrine`

### Option 2: Netlify (Gratuit)
1. Connectez votre repo GitHub
2. Netlify le déploiera automatiquement
3. Domaine personnalisé possible

### Option 3: Serveur VPS
1. Uploadez les fichiers via FTP/SCP
2. Configurez Nginx ou Apache
3. C'est prêt!

## 📝 Licence et Usage

Ce site est créé pour SkillBadge. Tous les contenus et designs sont propriétaires à SkillBadge.

---

## 💡 Prochaines Étapes

- [ ] Créer un dossier `assets/images/` et ajouter des images
- [ ] Intégrer un backend pour le formulaire de contact
- [ ] Ajouter plus d'articles blog réels
- [ ] Configurer les liens sociaux
- [ ] Ajouter Google Analytics
- [ ] Mettre en place un système de notification email
- [ ] Créer une page blog complète séparée
- [ ] Ajouter un système de newsletter

## 🆘 Problèmes Courants

### Le site n'apparaît pas correctement
- Vérifiez qu'HTML, CSS, et JS sont dans le même dossier
- Essayez avec un serveur local (ne pas juste ouvrir le fichier)
- Videz le cache navigateur (Ctrl+Shift+Del)

### Les liens n'activent pas les sections
- Vérifiez les `id` dans HTML correspondent aux `href`
- La classe `.container` doit entourer le contenu

### Le hamburger menu ne fonctionne pas
- Vérifiez que `script.js` est chargé avant `</body>`
- Ouvrez la console (F12) pour voir les erreurs

## 📞 Support

Pour des questions sur la personnalisation:
- Vérifiez la documentation HTML/CSS/JS standard
- Consultez W3Schools ou MDN Web Docs

Bon développement! 🚀

---

**Créé pour SkillBadge - Burkina Faso 🇧🇫**
