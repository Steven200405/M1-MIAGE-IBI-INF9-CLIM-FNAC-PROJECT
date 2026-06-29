# M1-MIAGE-IBI-INF9-CLIM-FNAC-PROJECT

## Objectif du sujet: Récupérer le catalogue de Cdiscount sur les "climatiseur portable" pour faire des analyses intéressantes

## Choix technique: Selenium
Pour quoi Selenium ? Nous avons choisi d'utiliser Selenium car le contenu du catalogue de Cdiscount est chargé en JavaScript. ## Ainsi, il n'est pas possible d'utiliser un parseur pour du contenu js dynamique. Ensuite, il n'existe pas d'API Cdiscount pour ## récupérer le catalogue de produits. 

## Plan de récolte de données
Récupération des div de produits qui se trouvent dans la classe "sc-11c3ifi-8". Ensuite, à travers cette div, nous allons récupérer des informations plus précises que nous souhaitons obtenir comme par exemple le prix, des mots-clés pour différencier climatiseur électrique ou ventilateur.

Passage à la page suivante: Pour être redirigé à la page suivante, il y a à chaque fin de page le bouton "Suivant". Cependant, étant donné que le bouton n'est pas cliquable sur Selenium, nous avons trouvé un contournement en changeant d'URL (qui est l'URL de la page suivante) lorsqu'on retrouve le bouton "Suivant" sur la page courante.

## Stratégie de nettoyage de données et Calcul

Lors de l'extraction des données en Excel, pour des soucis de performances avec Selenium, nous avons seulement une colonne avec le texte en brute. 
Nous avons procédé à l'utilisation d'un séparateur "\n" pour avoir les colonnes nécessaires, tout en traitant des cas particuliers comme les annonces sponsorisées, en promotion et les bon plans. 
On sépare également le prix avant et après réduction, et on calcule le taux de réduction.

## Analyse

Création de plusieurs représentations:
- Histogramme pour regarder le prix médian entre les produits sponsorisés vs non sponsorisés

## Conclusion

Nous avons cherché à réaliser un sujet qui est sensible en cette période de canicule. 
Ainsi, nous avons procédé à une extraction des produits disponibles dans le catalogue de CDiscount en cherchant les "climatiseur mobile".

Après une phase de nettoyage et calcul de données pour rendre les informations exploitables, nous nous sommes focalisées sur le prix des produits, s'ils sont sponsorisés, en promotion ou un bon plan.

Une conclusion faite est "les produits sponsorisés sont plus vendus plus chers que les produits non sponsorisés en analysant le prix médian".

Nous avons également cherché à savoir si plus un produit est cher plus sa réduction est faible et plus un produit en réduction est pas cher puis sa réduction est grande. Après une visualisation par un graphe, on peut identifier une courbe de tendance qui semble correspondre à notre hypothèse. Néanmoins, dû à un déséquilibre dans l'échantillon, l'hypothèse devra être vérifiée avec un meilleur échantillon.

