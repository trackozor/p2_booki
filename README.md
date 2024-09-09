# booki-starter-pack
<!-- 
    Projet : Booki
    Auteur : david kevin
    Date de création : 08/09/2024
    Dernière modification : 09/09/2024
    Version : 1.0
    Licence : MIT
    Description : Ce projet est une application web de réservation d'hébergements. Il contient la structure HTML et les styles CSS pour l'interface utilisateur responsive.
-->

# Booki - Documentation du projet

## Description

**Booki** est une application web qui permet aux utilisateurs de réserver des hébergements en ligne. Ce dépôt contient le fichier HTML ainsi que la feuille de styles CSS pour la page d'accueil de l'application. Le projet a été conçu pour être responsive et conforme aux meilleures pratiques de développement front-end.

Le but de ce projet est de proposer une interface simple et efficace pour afficher les hébergements et mettre en avant ceux qui sont les plus populaires.

## Structure HTML

Le fichier HTML `index.html` utilise une structure sémantique et respecte les bonnes pratiques de l'HTML5. Voici les principales sections de ce fichier :

### Bandeau normalisé

Un **bandeau normalisé** est placé en haut du fichier HTML. Il contient des informations sur le projet, telles que le nom de l'auteur, la date de création et les détails de la licence.

### Sections principales

1. **`<head>`** :
    - Contient les méta-informations nécessaires comme le charset UTF-8 et les balises de viewport pour assurer que la page est optimisée pour les appareils mobiles.
    - Liens vers les polices Google Fonts et les icônes Font Awesome pour ajouter des styles modernes à l'interface.

2. **`<body>`** :
    - La balise `<header>` contient l'en-tête de la page (actuellement vide mais extensible pour ajouter une barre de navigation ou un logo).
    - La balise `<main>` contient deux sections principales :
        - `hebergements` : Une section dédiée à la liste des hébergements disponibles.
        - `populaires` : Une section mettant en avant les hébergements les plus populaires, avec une présentation sous forme de cartes.
    - La balise `<footer>` contient le pied de page (actuellement vide mais prévue pour ajouter des liens utiles et d'autres informations).

3. **Accessibilité** :
    - Le fichier HTML inclut des attributs `aria-hidden` et des éléments comme `sr-only` pour améliorer l'accessibilité aux personnes utilisant des lecteurs d'écran.

## Structure CSS

Le fichier CSS `style.css` gère l'apparence et la mise en page de la page HTML. Voici quelques détails clés sur les styles utilisés :

### Variables CSS

Les variables CSS sont définies dans le sélecteur `:root` pour permettre une gestion centralisée des couleurs et faciliter les modifications futures :

```css
:root {
    --main-color: #0065FC;
    --main-bg-color: #F2F2F2;
    --filter-bg-color: #DEEBFF;
}
