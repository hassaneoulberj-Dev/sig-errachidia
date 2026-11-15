# Contribuer — SIG Errachidia

Ce guide aide à proposer des corrections reproductibles pour ce projet académique.

## Signaler un problème

Décrire le comportement observé, le résultat attendu et les étapes pour reproduire le problème. Indiquer les versions des outils utilisés et joindre un exemple minimal lorsque cela est possible.

## Vérifications adaptées au projet

- Indiquer le document MXD, la couche et le système de coordonnées concernés par un problème.
- Préserver les chemins relatifs entre `arcmap/` et `data/`, ainsi que tous les fichiers associés aux rasters GRID et shapefiles.
- Utiliser Git LFS pour les données : vérifier `git lfs ls-files` avant l’envoi et `git lfs pull` après clonage.
- Après un remplacement de couche, ouvrir les MXD concernés dans ArcMap et vérifier les sources, la projection, la symbologie et la légende.
- Mettre à jour les inventaires de `docs/` et expliquer si une couche masquée est réintroduite pour permettre un traitement.
- Accompagner chaque nouvel export de carte de ses sources et paramètres ; ne pas modifier silencieusement les classes ou les pondérations.

## Proposer une modification

Créer une branche dédiée, limiter chaque commit à un changement cohérent et décrire sa motivation. Dans la demande de fusion, préciser les vérifications réalisées, leur résultat et les limites restantes. Actualiser la documentation lorsque le comportement ou les prérequis changent.
