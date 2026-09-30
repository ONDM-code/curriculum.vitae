# Portfolio – Daniela Mylene OBIANG NDONG

Portfolio personnel en une seule page, en HTML et CSS, avec un peu de JavaScript pour le formulaire de contact. Le design reprend la maquette réalisée sur Canva.

## Sections

- **Accueil** : titre « PORTFOLIO », portrait, liens LinkedIn et GitHub
- **Moi** : présentation, badge « Étudiante en 2e année », carte de contact
- **Parcours** : éducation, certifications, compétences techniques, expériences détaillées, langues, centres d'intérêts, atouts
- **Projets** : projets en cours, de 2025 et de 2026
- **Échangeons** : formulaire de contact

## Structure du projet

```
.
├── index.html
├── README.md
└── assets/
    ├── photo-hero.jpg
    ├── photo-moi.jpg
    ├── photo-contact.jpg
    └── projets/
        ├── coeurious.png
        ├── jeu-textuel.png
        ├── quiz-stem.png
        ├── sonometre.png
        ├── dashboard.png
        ├── bibliotheque.png
        └── evenements.png
```

Les images ne sont pas fournies avec le code : il faut les ajouter dans `assets/` avec exactement ces noms. Tant qu'une image est absente, la zone reste vide (portraits) ou affiche une icône (cartes de projets).

## Lancer le site en local

Aucune installation n'est nécessaire : ouvrir `index.html` dans un navigateur suffit.

Pour un serveur local :

```bash
python -m http.server 8000
```

Puis aller sur http://localhost:8000.

## Personnaliser

### Couleurs

Les couleurs sont définies en haut du fichier, dans le bloc `:root` :

| Variable | Rôle |
|---|---|
| `--night` | fond principal (violet nuit) |
| `--night-deep` | fond des sections sombres et des cartes |
| `--lavender` | fond clair, texte des grands titres |
| `--violet` | titres sur fond clair |
| `--orange` | accent (boutons, contours, carte Expérience) |

### Polices

- Titres : [Unbounded](https://fonts.google.com/specimen/Unbounded)
- Texte : [Space Mono](https://fonts.google.com/specimen/Space+Mono)

Les polices et les icônes (Font Awesome) sont chargées depuis un CDN : une connexion internet est nécessaire pour les voir.

### Contenu

- **Ajouter un projet** : copier une balise `<article class="card">` dans le bon groupe (En cours, 2025 ou 2026), puis changer l'image, l'icône et le texte.
- **Projet « en cours »** : ajouter la classe `doing` à la carte (`class="card doing"`) pour lui donner l'ombre blanche.
- **Liens des réseaux sociaux** du projet Coeurious : remplacer les `href="#"` par les vrais liens.

## Formulaire de contact

Le site n'a pas de serveur : le bouton « Envoyer » ouvre l'application e-mail du visiteur avec l'objet et le message déjà remplis, à destination de `obiangndongdanielamylene@gmail.com`.

Pour recevoir les messages directement, on peut brancher le formulaire sur un service comme Formspree ou Netlify Forms.

## Mise en ligne

Avec GitHub Pages :

1. Envoyer le dossier sur un dépôt GitHub.
2. Dans **Settings → Pages**, choisir la branche `main` et le dossier racine `/`.
3. Le site est disponible à l'adresse `https://<utilisateur>.github.io/<depot>/`.

## Accessibilité

- Navigation au clavier avec focus visible
- Animation du chevron désactivée si le visiteur a demandé de réduire les animations
- Mise en page adaptée aux écrans mobiles
- Textes alternatifs sur les images

## Contact

- E-mail : danielandong@icloud.com
- LinkedIn : [linkedin.com/in/daniela-obiang-ndong](https://linkedin.com/in/daniela-obiang-ndong)
- GitHub : [github.com/ONDM-code](https://github.com/ONDM-code)
