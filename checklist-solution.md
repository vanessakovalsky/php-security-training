# Solutions rapide pour sécuriser les failles


## Injection HTML

### Failles exploitables

- Informations disponible
- Lancement de script JS pour éxécuter un keylogger par exemple 


### Solutions de protection

- htmlentities() ou htmlspechialchars() pour échapper tout HTML affiché 
- utilisé json.parse pour afficher un objet JSON


## Broken Authentication

### Failles exploitables

- Accès à un espace identifié avec les informations publique
- Contournement du captcha
- Oubli de mot de passe : permet de vérifier si un compte existe si on a l'info que l'utilisateur 
- Affichage du mot de passe en clair
- Session non detruite et/ou variable globale $_SESSION non vidée
- Mot de passe stocké en clair côté client ou côté serveur

### Solutions de protection

- ne pas mettre d'information dans le formulaire pouvant aider / donnant les informations de connexions
- ne pas valider le mot de passe côté client
- ne pas dire si l'utilisateur existe ou pas lors d'une réinitialisation de mot de passe -> dire que si le compte existe un mail est parti
- Ne jamais affiché un mot de passe en clair, ou l'envoyé par mail, envoyer un lien pour réinitialiser le mot de passe 
- Lors d'une deconnexion, vider la variable $_SESSION, on peut pour être sûr utiliser également la fonction session_destroy(), mais celle-ci est automatiquement appelé par PHP au bout de plusieurs minutes d'inactivité d'un utilisateur
- Penser à chiffrer les mots de passes quelque soit le stockage utilisé, pour cela utilisé de préférence un algoryhtme sécurisé type SHA-256 ou SHA-512, et penser à conserver la clé de salage utilisé pour pouvoir comparer le mot de passe à celui qui est stocké


## Configuration serveur 

### Failles exploitables

- Exécution de commande shell / php
- Affichage des répertoires / listes de fichiers
- Surutilisation du serveur pour faire tomber celui-ci
- Exploitation des droits systèmes / bdd

### Solutions de protection

- Configuration des variables du php.ini : desactivation des fonctions dangereuses et non nécessaires, sécurisation des temps d'execution, mémoire maximum...
- Configuration d'apache : empêcher l'attaquant de lister les répertoires, d'afficher les informations non nécessaire
- Configuration des utilisateurs systèmes / BDD et limitations de leurs permissions au strict minimum nécessaire