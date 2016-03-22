***
# Dashboard
***
## Historique projet

- **24/02/2016:** création du trinôme, choix du sujet et des jeux de données. 
- **29/02/2016:** amorce du projet sur ipython notebook. Mise en place du jeu de données et affichage du tableau (DataFrame).
- **02/03/2016:** création du graphique (histogrammes) avec des barres horizontal pour les années 2013 à 2015.
- **02/03/2016:** création du dépot GitHub avec le fichier Readme.md et Dashboard.md.
- **04/03/2016:** ajout des deux graphiques dont la normalisation des données.
- **05/03/2016:** début de mise en forme du jeu de données sur la géolocalisation des régions.
- **06/03/2016:** réussite de la mise en forme du jeu de données et affichage dans un DataFrame.
- **09/03/2016:** début de réalisation de la carte de France avec les densités de médecins par région avec ggplot.

## Suivi de projet

> #### 1. Date 02/03/2016

> Lors du choix du projet et des jeux de données, nous avons eu du mal à créer une problèmatique. C'est en tombant sur un site présentant des données sur les professions de santé que notre problématique est apparu.
  
>>  *Problématique: Quel est la densité de médecins selon la géolocalisation des régions entre les années 2013 et 2015 ?*

>  A partir de [Data DRESS Sante](http://www.data.drees.sante.gouv.fr), nous avons téléchargé 3 jeux de données. Nous nous sommes interessés notamment à ce [tableau] (http://www.data.drees.sante.gouv.fr/TableViewer/tableView.aspx?ReportId=1155) contenant la densité de médecins par région et département de 2013 à 2015. Grace ces éléments, nous avons mis en forme les jeux de données et créer des tableaux (DataFrame). Puis nous avons extrait les informations concernant la densité des généralistes (ou médecine générale) afin de pouvoir les analyser par la suite.
  
> Enfin nous avons fait notre premier graphique afin de visualiser la densité des médecins par région entre 2013 et 2015 : le graphique se présente à l'aide de barres horizontal (histogramme) associées à la valeur de densité de médecins de la region selon l'année.

> #### 2. Date 04/03/2016 
> Ajout de deux graphiques, le premier montre l'évolution de la densité au fil des années. Nous constatons ainsi que dans certaines régions le nombre de médecins par habitant baisse progressivement au fil des années, et dans d'autres régions il y'a une légère augmentation. Dans un deuxième temps, un graphique normalisé afin de visualiser selon une même norme l'évolution des médecins au cours des années.

> ### 3. Date 06/03/2016 
> Après avoir chercher des informations sur la documentation de pandas afin d'afficher notre jeu de données récupéré sur le site [Data Gouv] (https://www.data.gouv.fr/fr/datasets/listes-des-communes-geolocalisees-par-regions-departements-circonscriptions-nd/). Nous avons décidé de rectifier le fichier manuellement en corrigant les problèmes d'encoding pour les noms des regions et les chefs-lieu utile pour la réalisation de notre carte. Par le biais du package pandas, nous avons réussi après quelques difficultés à créer un jeu de données intéressant afin de pouvoir travailler dessus.

> une jointure de la table contenant la densité des médecins de 2013 à 2015 avec la table de géolocalisation des régions réalisée. Pour effectuer cette tache,  il a fallu créer une colonne distincte aux deux tableaux, c'est pourquoi un renommage des colonnes a été nécessaire. La jointure a pu ainsi se faire naturellement sur la colonne "Nom région".

> ### 4. Date 09/03/2016
> L'équipe s'est interessé à la librairie ggplot afin de réaliser une première itération d'une carte de la région française avec les densité de médecins.

> ### 4. Date 18/03/2016
> Abandon de ggplot, library non mature sur python.

> Nous avons utilisés la library Folium pour afficher une map avec les marqueurs sur les régions.

> Nous avons aussi créés une page HTML utilisant la library D3 + une geojson des régions de France pour afficher une carte avec les différentes densités.

## Problèmes rencontrées

- 1er jeu de données sur la géolocalisation des ambassades de France --> problème impossible de travailler dessus et mettre en place des méthodes de statistiques/ML.
- Jeu de données pour la géolocalisation des régions à partir des données venant de [Data Gouv](https://www.data.gouv.fr/fr/datasets/listes-des-communes-geolocalisees-par-regions-departements-circonscriptions-nd/), ce jeu de données n'est pas complet donc nous avons dû le modifier à l'aide de google map afin de compléter certaines latitude et longitude. 
- Le fichier CSV du jeu de données précédent avait un problème d'encodage des caractères.
- Difficulté pour installer ggplot, mais le problème venait du réseau de l'université ce qui supprimait la commande conda.exe après avoir tenté d'installer la librairie ggplot.
***
<p align="center"> © Copyright 2016 - Jérémie Chattou & Didier Bertille & Zacharie Barbecot </p>
