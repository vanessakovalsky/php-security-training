# Exercice 7 - Sessions 

Cet exercice a pour objectifs : 

* d'identifier les problèmatiques autour de la gestion des sessions
* de savoir se prémunir des attaques sur le serveur


## Exploitation des failles

* La première étapes va être de voir quel est le risque des bugs identifiés, à partir de la liste suivante, et de ce que vous connaissez / avez appris, identifier quels sont les risques sur les différentes pages de bugs et comment les exploiter :
    * Session Management - Administrative Portals,smgmt_admin_portal.php
    * Session Management - Cookies (HTTPOnly),smgmt_cookies_httponly.php
    * Session Management - Cookies (Secure),smgmt_cookies_secure.php
    * Session Management - Session ID in URL,smgmt_sessionid_url.php
    * Session Management - Strong Sessions,smgmt_strong_sessions.php
* Pour chaque bug, noter le résultat que vous obtenez et le risque que cela présente


## Protection contre les failles

* Maintenant que nous avons identifier différentes failles liées à la gestion des sessions, quelles solutions pouvez vous mettre en place pour chacune de ces failles afin de les prévenir ?