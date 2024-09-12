# booki-starter-pack
<!-- 
    Projet : Booki
    Auteur : david kevin
    Date de création : 08/09/2024
    Dernière modification : 12/09/2024
    Version : 2.0
    Licence : MIT
    Description : Ce projet est une application web de réservation d'hébergements. Il contient la structure HTML et les styles CSS pour l'interface utilisateur responsive.
-->

# Booki - Documentation du projet

## Description

**Booki** est une application web permettant aux utilisateurs de rechercher et réserver des hébergements et des activités dans différentes destinations touristiques. Le projet a été conçu avec une approche mobile-first pour garantir une expérience utilisateur fluide sur tous les appareils, qu'il s'agisse de smartphones, tablettes ou ordinateurs de bureau. 

Le projet présente une interface moderne, intuitive et responsive, avec une gestion centralisée des styles via des variables CSS. Ce dépôt contient la structure HTML et les styles CSS pour la page d'accueil de l'application.

## Fonctionnalités

- **Recherche d'hébergements** : Un champ de recherche permet aux utilisateurs de trouver des logements dans une ville spécifique (par exemple : "Marseille, France").
- **Filtres** : Des filtres permettent de trier les hébergements selon des critères tels que l'option économique, familial, romantique, ou les "pépites".
- **Affichage des hébergements** : Les hébergements sont présentés sous forme de cartes incluant une image, un titre, un prix et une note.
- **Section populaire** : Une section dédiée affiche les hébergements les plus populaires.
- **Activités** : Une section répertorie les activités disponibles dans la ville recherchée.
- **Responsivité** : Le site est entièrement responsive et optimisé pour les appareils mobiles.
- **Accessibilité** : Le projet inclut des optimisations pour les lecteurs d'écran avec l'utilisation d'attributs ARIA et des classes spécifiques comme `sr-only`.

## Technologies

- **HTML5** : Structure sémantique et compatible avec les moteurs de recherche.
- **CSS3** : Styles modernes avec gestion des variables, Flexbox pour la disposition, et Media Queries pour la responsivité.
- **Google Fonts** : Utilisation de la police **Raleway** pour une typographie moderne et épurée.
- **Font Awesome** : Icônes vectorielles pour améliorer la présentation visuelle.

## Structure du projet

### Fichiers principaux

- `index.html` : Contient la structure HTML de la page d'accueil.
- `style.css` : Feuille de styles qui gère l'apparence et la mise en page.
- `images/` : Dossier contenant les images utilisées pour illustrer les hébergements et les activités.

### Arborescence du projet

booki/
├── css/
│   └── style.css       # Feuille de style principale
├── images/
│   ├── logo/           # Contient le logo de l'application
│   ├── hebergements/   # Images des hébergements
│   └── activites/      # Images des activités
└── index.html          # Fichier HTML principal

### Structure HTML

Le fichier index.html utilise une structure HTML sémantique pour garantir une lisibilité optimale par les moteurs de recherche et améliorer l'accessibilité.
Sections principales
# head :

Déclaration des métadonnées essentielles, comme le charset UTF-8, la description de la page et la balise viewport pour la responsivité.
Lien vers les polices Google Fonts et les icônes Font Awesome.
Lien vers la feuille de styles style.css.
# header :

Contient le logo de Booki ainsi que le menu de navigation permettant d'accéder aux sections principales de la page, telles que les hébergements et les activités.
# main :

Barre de recherche : Un formulaire permet aux utilisateurs de saisir une localisation pour rechercher des hébergements.
Filtres : Des boutons de filtres permettent de trier les résultats en fonction de critères spécifiques (ex : économique, familial, romantique, etc.).
Section Hébergements : Présente une liste d'hébergements sous forme de cartes avec une image, un titre, un prix et une note.
Section Populaires : Une section dédiée aux hébergements populaires avec les mêmes éléments de présentation que les autres hébergements.
Section Activités : Répertorie les activités disponibles dans la ville sélectionnée.
# footer :

Contient plusieurs menus de navigation vers des sections importantes comme "À propos", "Nos hébergements", et "Assistance".
Structure CSS
Le fichier style.css applique des styles globaux en utilisant des variables CSS pour faciliter la personnalisation et la maintenance du projet.

### Variables CSS
Les variables globales sont définies dans le sélecteur :root, ce qui permet de centraliser les couleurs et d'autres valeurs réutilisables.
:root {
    --main-color: #0065FC;        /* Couleur principale */
    --main-bg-color: #F2F2F2;     /* Couleur de fond principale */
    --filter-bg-color: #DEEBFF;   /* Couleur de fond des filtres */
    --font-weight: 700;           /* Poids des polices */
}
## Styles globaux
Police : La police Raleway est utilisée pour l'ensemble de la page pour assurer une apparence moderne et cohérente.
Flexbox : Utilisé pour gérer la disposition des éléments, notamment pour centrer ou espacer les sections.
Responsivité : Grâce aux Media Queries, le contenu s'adapte en fonction de la taille de l'écran.
Cartes : Les hébergements et les activités sont présentés sous forme de cartes avec des coins arrondis et des ombres pour un effet visuel agréable.
Exemples de styles
Barre de navigation :
.nav {
    display: flex;
    justify-content: center;
    gap: 30%;
}
.nav-element:hover {
    color: var(--main-color);
    border-top: 2px solid var(--main-color);
}
# Cartes d'hébergements :
.card {
    background-color: white;
    border-radius: 1.25rem;
    padding: 0.3125rem;
    filter: drop-shadow(0 0.1875rem 0.9375rem rgba(0, 0, 0, 0.1));
}
.card img {
    object-fit: cover;
    border-top-left-radius: 1.25rem;
    border-top-right-radius: 1.25rem;
}
### Media Queries
Des Media Queries sont utilisées pour garantir que l'interface s'adapte parfaitement aux différents écrans.
@media (max-width: 64rem) {
    .hebergements-and-populaires {
        flex-direction: column;
    }
    .hebergements, .populaires {
        width: 80%;
    }
}
### Accessibilité
ARIA : Des attributs aria-hidden et sr-only sont utilisés pour rendre le contenu accessible aux lecteurs d'écran.
Icônes : Les icônes sont accompagnées d'un texte alternatif (alt) pour décrire leur fonction aux utilisateurs de lecteurs d'écran.
Installation
Clonez ce dépôt sur votre machine locale avec la commande suivante :git clone https://github.com/votre-utilisateur/booki.git
Ouvrez le fichier index.html dans votre navigateur pour afficher la page d'accueil.

