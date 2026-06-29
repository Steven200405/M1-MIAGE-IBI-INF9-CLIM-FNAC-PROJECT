# M1-MIAGE-IBI-INF9-CLIM-FNAC-PROJECT

# Objectif du sujet: Récupérer le catalogue de Cdiscount sur les "climatiseur portable" pour faire des analyses intéressantes

# Choix technique: Selenium
## Pour quoi Selenium ? Nous avons choisi d'utiliser Selenium car le contenu du catalogue de Cdiscount est chargé en JavaScript. ## Ainsi, il n'est pas possible d'utiliser un parseur pour du contenu js dynamique. Ensuite, il n'existe pas d'API Cdiscount pour ## récupérer le catalogue de produits. 

# Plan de récolte de données
## Récupération des div de produits qui se trouvent dans la classe "sc-11c3ifi-8". Ensuite, à travers cette div, nous allons récupérer des informations plus précises que nous souhaitons obtenir comme par exemple le prix, des mots-clés pour différencier climatiseur électrique ou ventilateur.

## Passage à la page suivante: Pour être redirigé à la page suivante, il y a à chaque fin de page le bouton "Suivant". Cependant, étant donné que le bouton n'est pas cliquable sur Selenium, nous avons trouvé un contournement en changeant d'URL (qui est l'URL de la page suivante) lorsqu'on retrouve le bouton "Suivant" sur la page courante.

# Stratégie de nettoyage de données



# Calcul

# Analyse

# Conclusion
