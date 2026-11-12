# UNDERWAVE

Site de l'association UNDERWAVE, association culturelle et sociale à Marseille.

Site statique (un seul fichier `index.html` + images dans `img/`), publié avec GitHub Pages.

## Structure

- `index.html` : toutes les pages du site (Accueil, Projets, OPN, Espaces Partagés, ALT MEDIA, Actions solidaires, Contact & infos), affichées selon l'adresse (`#projets`, `#opn`…).
- `img/` : photos et affiches.
- `assets/logo/` : versions du logo.

## Charte

- Lime `#DEFE52`, magenta `#EA33D2`, noir, blanc.
- Une seule typo : Inter Tight.
- Style inspiré de noideas.website.

## Règle de contenu

Les textes reprennent mot pour mot ceux de l'association : ne pas les réécrire ni les résumer sans accord.

## Espaces Partagés

Le dossier `espaces-partages/` contient le répertoire culturel collaboratif Espaces Partagés, publié à l'adresse `/underwave-site/espaces-partages/`.

- `index.html` : tout le site (pages, styles et code).
- `vendor/` : bibliothèques hébergées sur le site (carte Leaflet, client Supabase, police Inter Tight), pour qu'aucun service tiers ne reçoive l'adresse des visiteurs.
- `supabase/` : structure de la base de données (comptes, lieux, annonces, messages, signalements). À exécuter dans l'éditeur SQL de Supabase : `schema.sql`, puis `02-complements.sql`.

Les comptes et les données sont gérés par Supabase (région Paris). La clé présente dans `index.html` est la clé publique : les règles d'accès sont appliquées par la base elle-même.
