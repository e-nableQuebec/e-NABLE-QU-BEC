# e-NABLE Quebec - Site GitHub Pages

Site vitrine statique pour e-NABLE Quebec, heberge sur GitHub Pages.

## Objectif du site
- Presenter la mission e-NABLE Quebec.
- Permettre aux visiteurs de:
  - Demander une prothese.
  - Rejoindre l'equipe benevole.
  - Contacter l'organisation.
- Mettre en valeur les membres, partenaires et activites.

## Structure du projet
- `index.html`: structure et contenu principal de la page.
- `assets/css/styles.css`: styles visuels (couleurs, mise en page, responsive).
- `assets/js/main.js`: logique interactive (langue, carrousel, filtres membres, modale).
- `assets/`: images et icones utilisees par la page.

## Comment fonctionne la page
### 1) Contenu et sections
Le fichier `index.html` contient les grandes sections:
- Hero (intro)
- Mission
- Participer
- Membres
- Contact
- Partenaires

### 2) Style et responsive
- Le design est defini dans `assets/css/styles.css`.
- Les medias queries adaptent la page pour mobile, tablette et desktop.

### 3) Interactions JavaScript
Le fichier `assets/js/main.js` gere:
- Le basculement FR/EN via `translations` et `setLanguage()`.
- Les animations d'apparition (`IntersectionObserver`).
- Le carrousel de galerie (boutons + auto-defilement).
- Le carrousel/filtres des membres.
- L'ouverture/fermeture de la fenetre modale membre.
- Le scroll doux vers les sections ancrees.

## Guide simple pour non-techniques
### Modifier un texte
1. Ouvrir `index.html` pour le texte statique.
2. Ouvrir `assets/js/main.js` pour les textes bilingues (objet `translations`).
3. Sauvegarder et publier les changements.

### Modifier une image
1. Remplacer l'image dans `assets/` (meme nom de fichier de preference).
2. Si le nom change, mettre a jour le chemin dans `index.html` ou `assets/js/main.js`.

### Ajouter un membre
1. Ouvrir `assets/js/main.js`.
2. Dans le tableau `members`, ajouter un objet avec:
   - `name`
   - `role_fr`
   - `role_en`
   - `photo`
   - `link`
3. Sauvegarder.

### Modifier les liens formulaires
Mettre a jour les attributs `href` des boutons dans la section Participer de `index.html`.

## Publication GitHub Pages
Le site est statique. Toute modification poussee sur la branche de publication configuree dans GitHub Pages est deployee automatiquement par GitHub.

## Bonnes pratiques recommandees
- Garder les noms de fichiers stables pour eviter les liens casses.
- Eviter les espaces dans les noms de fichiers image.
- Tester rapidement en mobile et desktop apres modification.
- Mettre a jour les textes FR et EN en meme temps pour garder la coherence.
