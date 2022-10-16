# Exercice 5 - Injection SQL

Cet exercice a pour objectifs : 

* d'identifier les problèmatiques autour de l'injection SQL
* de savoir se prémunir des attaques sur le serveur


## Exploitation des failles

* La première étapes va être de voir quel est le risque des bugs identifiés, à partir de la liste suivante, et de ce que vous connaissez / avez appris, identifier quels sont les risques sur les différentes pages de bugs et comment les exploiter :
    * SQL Injection (GET/Search),sqli_1.php
    * SQL Injection (GET/Select),sqli_2.php
    * SQL Injection (POST/Search),sqli_6.php
    * SQL Injection (POST/Select),sqli_13.php
    * SQL Injection (AJAX/JSON/jQuery),sqli_10-1.php
    * SQL Injection (CAPTCHA),sqli_9.php
    * SQL Injection (Login Form/Hero),sqli_3.php
    * SQL Injection (Login Form/User),sqli_16.php

* Pour chaque bug, noter le résultat que vous obtenez et le risque que cela présente


## Protection contre les failles

* Maintenant que nous avons identifier différentes failles liées à l'injection SQL, quelles solutions pouvez vous mettre en place pour chacune de ces failles afin de les prévenir ?