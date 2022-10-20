# Exercice 2 - Gestion des mots de passes

Cet exercice a pour objectifs : 

* d'identifier les problèmatiques autour de la gestion des mots de passe
* de savoir se prémunir des attaques sur les identifiants


## Exploitation des failles

* La première étapes va être de voir quel est le risque des bugs identifiés, à partir de la liste suivante, et de ce que vous connaissez / avez appris, identifier quels sont les risques sur les différentes pages de bugs et comment les exploiter :
    * Broken Authentication - CAPTCHA Bypassing,ba_captcha_bypass.php
    * Broken Authentication - Forgotten Function,ba_forgotten.php
    * Broken Authentication - Insecure Login Forms,ba_insecure_login.php
    * Broken Authentication - Logout Management,ba_logout.php
    * Broken Authentication - Password Attacks,ba_pwd_attacks.php
    * Broken Authentication - Weak Passwords,ba_weak_pwd.php
    * Base64 Encoding (Secret),insecure_crypt_storage_3.php

* Pour chaque bug, noter le résultat que vous obtenez et le risque que cela présente

<details>
    <summary>De l'aide pour Hacker ?</summary>
    - https://medium.com/@grep_security/broken-authentication-and-session-management-part-%E2%85%B0-50e760c9f599 
    
    - https://infosecgirls.gitbook.io/infosecgirls-training/v/appsec/web-application-pentesting/a2-broken-authentication-and-session/broken-authentication-with-bwapp

    - 
</details>

## Protection contre les failles

* Maintenant que nous avons identifier différentes failles liées à la sécurité des identifiants, quelles solutions pouvez vous mettre en place pour chacune de ces failles afin de les prévenir ?