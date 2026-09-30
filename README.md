# SunuGox

> Civic-tech sénégalaise pour piloter le cycle complet des signalements urbains.

## Produit

SunuGox relie trois espaces autour d'un même dossier opérationnel :

**Citoyen → Mairie → Agent terrain → Inspection → Intervention → Contre-visite → Clôture**

Les exemples de démonstration utilisent Dakar, Pikine, Guédiawaye, Yeumbeul, Parcelles Assainies et Grand-Yoff.

## Expérience

Le dossier est l'objet central. Chaque rôle retrouve les mêmes informations métier avec une interface adaptée à son travail :

- citoyen : déclarer, localiser, suivre ;
- mairie : qualifier, affecter, planifier, contrôler ;
- agent : exécuter la mission, documenter le terrain, confirmer l'intervention.

Le prototype inclut navigation, changement de rôle, recherche, filtres, dossiers, timeline, formulaire, notifications, états d'action et responsive desktop/mobile.

## Architecture

~~~text
SunuGox/
├── index.html
├── data/
│   └── demo.js
├── scripts/
│   └── app.js
└── styles/
    └── app.css
~~~

La séparation est volontairement simple pour ce prototype front-end :

- data/ contient les données de démonstration ;
- scripts/ contient l'état applicatif et les interactions ;
- styles/ contient le système visuel ;
- index.html est le point d'entrée.

## Direction visuelle

SunuGox possède sa propre identité : surfaces claires, encre bleu nuit, accent terre cuite, typographie Space Grotesk + DM Sans, timeline opérationnelle, cartographie stylisée et responsive mobile.

Aucun composant, layout, CSS, navigation ou logique visuelle de Laravel-group n'est utilisé comme base.

## Lancer

Le projet est un site statique ES modules. Un serveur HTTP local est recommandé :

~~~bash
python3 -m http.server 8000
~~~

Puis ouvrir http://localhost:8000.

## Suite

Le prochain niveau consiste à remplacer data/demo.js par une API persistante, puis à brancher authentification, stockage des photos, géolocalisation réelle, notifications et historique immuable.
