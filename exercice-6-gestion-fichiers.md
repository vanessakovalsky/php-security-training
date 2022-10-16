# Exercice 6 - Gestion des fichiers

Cet exercice a pour objectifs : 

* d'identifier les problèmatiques autour de la gestion des fichiers
* de savoir se prémunir des attaques sur le serveur


## Exploitation des failles

* La première étapes va être de voir quel est le risque des bugs identifiés, à partir de la liste suivante, et de ce que vous connaissez / avez appris, identifier quels sont les risques sur les différentes pages de bugs et comment les exploiter :
    * Directory Traversal - Directories,directory_traversal_2.php?directory=documents
    * Directory Traversal - Files,directory_traversal_1.php?page=message.txt
    * Restrict Device Access,restrict_device_access.php
    * Restrict Folder Access,restrict_folder_access.php
    * Unrestricted File Upload,unrestricted_file_upload.php

* Pour chaque bug, noter le résultat que vous obtenez et le risque que cela présente


## Protection contre les failles

* Maintenant que nous avons identifier différentes failles liées à la gestion des fichiers, quelles solutions pouvez vous mettre en place pour chacune de ces failles afin de les prévenir ?