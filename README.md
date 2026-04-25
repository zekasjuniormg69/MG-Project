# 📱 G-Kub - Site E-commerce Professionnel

Bienvenue dans le projet **G-Kub**, un site vitrine e-commerce moderne, fluide et professionnel développé en HTML et CSS.

---

## 📋 Table des Matières

1. [Description du Projet](#description-du-projet)
2. [Structure du Dossier](#structure-du-dossier)
3. [Fonctionnalités](#fonctionnalités)
4. [Palette de Couleurs](#palette-de-couleurs)
5. [Comment Utiliser](#comment-utiliser)
6. [Guide pour Développeurs Juniors](#guide-pour-développeurs-juniors)
7. [Évolutions Futures](#évolutions-futures)
8. [Support et Contact](#support-et-contact)

---

## 📝 Description du Projet

**G-Kub** est un site vitrine professionnel conçu pour présenter et vendre des produits premium. Le site est entièrement responsive et fonctionne parfaitement sur tous les appareils (desktop, tablette, mobile).

**Caractéristiques principales:**
- ✅ Design moderne et épuré
- ✅ Navigation fluide et intuitive
- ✅ Responsive design (mobile-first)
- ✅ Code bien commenté et structuré
- ✅ Footer communicant avec informations de contact

---

## 📁 Structure du Dossier

```
Site E-commerce 1/
│
├── index.html              # Page principale (à ne pas modifier)
├── text.txt                # Fichier de requirements (ce projet)
├── README.md              # Ce fichier de documentation
│
├── css/
│   └── style.css          # Feuille de styles principale
│
├── images/
│   ├── logo.png           # Logo du site (à ajouter)
│   ├── produit1.png       # Image du produit 1 (à ajouter)
│   ├── produit2.png       # Image du produit 2 (à ajouter)
│   └── produit3.png       # Image du produit 3 (à ajouter)
│
└── js/                     # Dossier pour les futures extensions JavaScript
```

---

## ✨ Fonctionnalités

### En-tête (Header)
- Logo avec nom de marque
- Navigation principale avec liens vers:
  - Accueil
  - Produits
  - Contact
- Design sticky (reste en haut lors du scroll)

### Section Accueil (Hero)
- Bannière d'introduction attractive
- Appel à l'action "Voir nos produits"
- Gradient de couleurs professionnel

### Section Produits
- Grille responsive (3 colonnes → 2 → 1 selon la résolution)
- Cartes produits avec:
  - Image du produit
  - Titre et description
  - Prix
  - Bouton "Acheter"
- Effets visuels au survol (hover)

### Pied de Page (Footer)
- Section "À propos" - description de l'entreprise
- Section "Liens rapides" - navigation importante
- Section "Contact" - informations de contact:
  - Email cliquable
  - Téléphone cliquable
  - Adresse physique
- Barre de copyright

---

## 🎨 Palette de Couleurs

Le projet utilise une palette de couleurs professionnelle et cohérente:

| Variable CSS | Couleur | Utilisation |
|---|---|---|
| `--couleur-primaire` | #2c3e50 (Bleu-gris) | En-tête, footer, textes principaux |
| `--couleur-secondaire` | #3498db (Bleu clair) | Accents, hovers |
| `--couleur-accent` | #e74c3c (Rouge) | Boutons d'action, prix |
| `--couleur-fond` | #ecf0f1 (Gris très clair) | Fond de page |
| `--couleur-blanc` | #ffffff | Cartes, texte sur fond sombre |

> 💡 **Conseil:** Pour modifier les couleurs globalement, changez les variables CSS dans le fichier `style.css` (lignes 20-30).

---

## 🚀 Comment Utiliser

### 1. Installation
Aucune installation requise! Le projet fonctionne directement dans un navigateur.

### 2. Ouverture du Site
- Double-cliquez sur `index.html`
- Ou faites un clic droit → "Ouvrir avec" → votre navigateur préféré

### 3. Ajouter les Images
1. Préparez vos images:
   - `logo.png` - Logo de votre entreprise
   - `produit1.png`, `produit2.png`, `produit3.png` - Photos des produits
2. Placez-les dans le dossier `images/`
3. Les images s'afficheront automatiquement dans le site

### 4. Modifier les Informations
Pour adapter le site à votre entreprise:

**Entreprise et textes:**
- Ouvrez `index.html`
- Modifiez:
  - Le titre dans `<h1>G-Kub</h1>` (ligne 24)
  - Les noms et descriptions des produits
  - Les informations de contact dans le footer

**Couleurs:**
- Ouvrez `css/style.css`
- Modifiez les variables CSS (lignes 20-30)

**Informations de Contact (Footer):**
- Email: remplacez `contact@gkub.com`
- Téléphone: remplacez `+33 (0) 1 23 45 67 89`
- Adresse: remplacez `123 rue du Commerce, 75000 Paris`

---

## 📚 Guide pour Développeurs Juniors

### Comprendre la Structure HTML

**Zones principales:**
```
header        → Navigation et logo
hero         → Section d'accueil
produits     → Grille de produits
footer       → Informations et contact
```

### Points Clés CSS à Comprendre

#### 1. **Variables CSS** (lignes 20-30)
Les variables CSS permettent de définir des valeurs réutilisables:
```css
--couleur-primaire: #2c3e50;
/* Utilisation: color: var(--couleur-primaire); */
```

#### 2. **Flexbox** - Pour aligner des éléments
```css
display: flex;
justify-content: space-between;  /* Espace entre les éléments */
align-items: center;             /* Aligne verticalement */
```

#### 3. **Grid** - Pour les grilles de produits
```css
display: grid;
grid-template-columns: repeat(3, 1fr);  /* 3 colonnes égales */
gap: 30px;                               /* Espacement entre éléments */
```

#### 4. **Media Queries** - Pour le responsive
```css
@media (max-width: 768px) {
    /* Styles pour les écrans ≤ 768px */
    .produits-grid {
        grid-template-columns: repeat(2, 1fr);  /* 2 colonnes au lieu de 3 */
    }
}
```

#### 5. **Transitions et Hover** - Pour les animations
```css
transition: all 0.3s ease;  /* Animation fluide */
.element:hover {
    transform: translateY(-8px);  /* Mouvement au survol */
    box-shadow: 0 4px 16px rgba(0, 0, 0, 0.15);
}
```

### Bonnes Pratiques Observées

✅ **Code bien commenté:** Chaque section est commentée en français  
✅ **Variables réutilisables:** Couleurs et espacements centralisés  
✅ **Structure sémantique:** Utilisation de balises HTML appropriées  
✅ **Responsive Design:** Fonctionne sur tous les appareils  
✅ **Nommage cohérent:** Classes avec tirets (BEM-like)

### Comment Ajouter une Nouvelle Fonctionnalité

Exemple: Ajouter un produit 4ème

1. **Dans `index.html`** (copier/coller le bloc produit):
```html
<!-- Produit 4 -->
<div class="produit-card">
    <div class="produit-image">
        <img src="images/produit4.png" alt="Produit 4 - G-Kub">
    </div>
    <div class="produit-info">
        <h3>Produit Premium 4</h3>
        <p class="produit-description">Description du produit...</p>
        <div class="produit-footer">
            <span class="prix">99,99€</span>
            <button class="btn-acheter">Acheter</button>
        </div>
    </div>
</div>
```

2. **Ajouter l'image** `produit4.png` dans le dossier `images/`

3. **Adapter le CSS si nécessaire:**
```css
@media (max-width: 768px) {
    .produits-grid {
        grid-template-columns: repeat(2, 1fr);  /* Ou repeat(4, 1fr) pour 4 colonnes */
    }
}
```

---

## 🔄 Évolutions Futures

Le site est prêt pour les améliorations suivantes:

### Phase 2 - Interactivité (JavaScript)
- [ ] Panier d'achat fonctionnel
- [ ] Filtre de produits par catégorie
- [ ] Effet de défilement parallaxe
- [ ] Formulaire de contact avec validation
- [ ] Slider d'images/testimonials

### Phase 3 - Backend & E-commerce
- [ ] Base de données des produits
- [ ] Système de paiement
- [ ] Gestion des commandes
- [ ] Compte utilisateur
- [ ] Système d'avis clients

### Phase 4 - SEO & Performance
- [ ] Optimisation SEO
- [ ] Compression des images
- [ ] Minification du CSS
- [ ] Service Workers (Progressive Web App)

---

## 📞 Support et Contact

### Pour Modifier le Site
1. **Textes/Images:** Modifiez directement les fichiers HTML
2. **Couleurs:** Changez les variables dans `style.css`
3. **Layout:** Ajustez les propriétés CSS flexbox/grid
4. **Contact:** Mettez à jour les informations dans le footer

### Points de Contact (à personnaliser)
- 📧 Email: `contact@gkub.com`
- 📞 Téléphone: `+33 (0) 1 23 45 67 89`
- 📍 Adresse: `123 rue du Commerce, 75000 Paris`

---

## 📄 Licence

Ce projet est fourni à titre d'exemple. Libre d'utilisation et de modification.

---

**Créé avec ❤️ pour G-Kub**  
*Site professionnel et moderne prêt à la production*

Version: 1.0  
Dernière mise à jour: 25 Avril 2026
