# Exercice 1 - Sécurité côté client

Cet exercice a pour objectifs : 

* de découvrir l'environnement utilisé pendant la formation
* de savoir sécuriser un site côté client

## Pré-requis

* Afin d'installer l'application web, un environnement PHP / SQL est requis, si vous nous n'en avez pas vous pouvez utiliser XAMPP (multi-plateforme) : https://www.apachefriends.org/fr/index.html
* Un éditeur de code configuré pour PHP est requis, nous utiliserons VisualStudioCode (https://code.visualstudio.com/) , mais cela peut être celui avec lequel vous êtes le plus à l'aise 

## Présentation de l'application et installation

* Afin de manipuler les principales failles de sécurité et de voir comment les corriger, nous allons installer une application web écrite en PHP qui présente de nombreux bugs. Il s'agit de l'application bWAPP (http://www.itsecgames.com)
* Afin de l'installer, télécharger l'archive ZIP à l'adresse : http://www.itsecgames.com/download.htm et décompresser l'archive dans votre environnement PHP
* Vous pouvez également si vous êtes familier de virtual Box, télécharger une VM prête à l'emploi à cette adresse : https://sourceforge.net/projects/bwapp/files/bee-box/ 
* extraire le dossier bWAPP dans votre dossier de serveur web (exemple /var/www/html)
* Donner les droits complets sur les dossiers 'passwords', 'images', 'documents' et 'logs'. 
* Modifier le fichier admin/settings.php pour renseigner vos informations de connexion à votre base de données
* Aller sur le site dans un navigateur et appelé la page install.php
* Cliquer sur 'here' pour installer bWAPP. Cela créera la structure de la base de données et la remplira
* Aller sur la page de connexion: 	exemple: http://localhost/bWAPP/login.php
* Se connecter avec les identifiants par défaut ou créer un nouvel utilisateur
    * identifiants par défaut : bee/bug
* Vous êtes prêt à utiliser l'application

## Exploitation des failles

* La première étapes va être de voir quel est le risque des bugs identifiés, à partir de la liste suivante, et de ce que vous connaissez / avez appris, identifier quels sont les risques sur les différentes pages de bugs et comment les exploiter :
    * HTML Injection - Reflected (GET),htmli_get.php
    * HTML Injection - Reflected (POST),htmli_post.php
    * HTML Injection - Reflected (Current URL),htmli_current_url.php
    * HTML Injection - Stored (Blog),htmli_stored.php
    * Cross-Site Scripting - Reflected (AJAX/JSON),xss_ajax_2-1.php

* Pour chaque bug, noter le résultat que vous obtenez et le risque que cela présente

<details>
    <summary>De l'aide pour Hacker ?</summary>
    - https://jaiguptanick.github.io/Blog/blog/Walkthrough_of_bWAPP_solutions_A1_injection_writeups/ 
    
    - https://hackbotone.com/cross-site-scripting-reflected-ajax-json-b280c1777e88 
</details>

## Protection contre les failles

* Maintenant que nous avons identifier différentes failles liées à la sécurité côté client, quelles solutions pouvez vous mettre en place pour chacune de ces failles afin de les prévenir ?
