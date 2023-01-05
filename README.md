# TP3 : Docker

## Exercice 

Préparer un fichier docker-compose.yml permettant de créer un environnement de développement Web PHP.

Vous devrez avoir les services suivants :

* Apache
* PHP
* Mysql
* phpmyadmin

Une fois votre environnement docker démarré, vous devez être capable de développer de nouvelles lignes de codes et de les voir en action sans faire de nouvelles actions sur votre environnement Docker

## Solution
* Créer et configurer le docker-compose.yml
* Lancer le docker-compose : 
```
docker compose up -d
```
* Créer et configurer un fichier index.php dans /opt/apache2
```
vim /opt/apache2/index.php

<html>
    <head>
        <title>PHP Test</title>
    </head>
    <body>
        <?php 
            echo '<p>Hello World</p>';
            phpinfo(); ?>
    </body>
</html>
```
* Vérifier que la page est bien accessible
![](https://i.imgur.com/MNi926E.png)

* Vérifier que phpmyadmin est bien accessible
![](https://i.imgur.com/fEe8Qkt.png)


