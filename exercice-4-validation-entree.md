# Exercice 4 - Validation des entrées

Cet exercice a pour objectifs : 

* d'identifier les problèmatiques autour de la validation des entrées
* de savoir se prémunir des attaques sur le serveur


## Exploitation des failles

* La première étapes va être de voir quel est le risque des bugs identifiés, à partir de la liste suivante, et de ce que vous connaissez / avez appris, identifier quels sont les risques sur les différentes pages de bugs et comment les exploiter :
    * Unvalidated Redirects & Forwards (1),unvalidated_redir_fwd_1.php
    * Unvalidated Redirects & Forwards (2),unvalidated_redir_fwd_2.php
    * Client-Side Validation (Password),cs_validation.php
    * Cross-Site Scripting - Reflected (POST),xss_post.php

* Pour chaque bug, noter le résultat que vous obtenez et le risque que cela présente


## Protection contre les failles

* Maintenant que nous avons identifier différentes failles liées à la sécurité de la validation des entrées, quelles solutions pouvez vous mettre en place pour chacune de ces failles afin de les prévenir ?