# Commandes BASH

## Navigation dans le système de fichiers

| Commande | Description                              |
| -------- | ---------------------------------------- |
| `pwd`    | Affiche le chemin du répertoire courant  |
| `ls`     | Liste les fichiers/répertoires           |
| `ls -l`  | Liste détaillée (permissions, taille...) |
| `ls -a`  | Affiche aussi les fichiers cachés        |
| `cd`     | Change de répertoire                     |
| `cd ..`  | Remonte d’un niveau                      |
| `cd ~`   | Va dans le répertoire personnel          |
| `cd -`   | Revient au répertoire précédent          |
| `tree`   | Affiche l’arborescence des fichiers      |

## a Manipulation de fichiers et de répertoires

| Commande                  | Description                                 |
| ------------------------- | ------------------------------------------- |
| `touch fichier.txt`       | Crée un fichier vide                        |
| `mkdir mon_dossier`       | Crée un dossier                             |
| `cp source dest`          | Copie un fichier                            |
| `cp -r dossier1 dossier2` | Copie un dossier                            |
| `mv source dest`          | Déplace ou renomme un fichier/dossier       |
| `rm fichier.txt`          | Supprime un fichier                         |
| `rm -r dossier`           | Supprime un dossier et son contenu          |
| `rm -rf dossier`          | Supprime récursivement et sans confirmation |
| `stat fichier`            | Donne des infos détaillées sur un fichier   |

## Visualisation et recherche

| Commande                       | Description                             |
| ------------------------------ | --------------------------------------- |
| `cat fichier.txt`              | Affiche le contenu d’un fichier         |
| `less fichier.txt`             | Affiche avec navigation (page par page) |
| `more fichier.txt`             | Similaire à `less`                      |
| `head -n 10 fichier.txt`       | Affiche les 10 premières lignes         |
| `tail -n 10 fichier.txt`       | Affiche les 10 dernières lignes         |
| `tail -f fichier.txt`          | Suit un fichier en temps réel (logs)    |
| `grep "mot" fichier.txt`       | Cherche une chaîne dans un fichier      |
| `grep -r "mot" dossier`        | Recherche récursive                     |
| `find /chemin -name "fichier"` | Recherche un fichier par nom            |
| `locate nom_fichier`           | Recherche rapide via base de données    |

## Utilitaires système

| Commande                   | Description                        |
| -------------------------- | ---------------------------------- |
| `man commande`             | Affiche le manuel de la commande   |
| `history`                  | Affiche l’historique des commandes |
| `clear`                    | Nettoie l’écran                    |
| `chmod 755 fichier`        | Modifie les permissions            |
| `chown user:group fichier` | Change le propriétaire             |
| `df -h`                    | Espace disque disponible           |
| `du -sh dossier`           | Taille d’un dossier                |
| `top` / `htop`             | Affiche les processus en cours     |
| `ps aux`                   | Liste les processus                |
| `kill PID`                 | Termine un processus par ID        |
| `killall nom`              | Termine tous les processus nommés  |

## Archivage et compression

| Commande                          | Description                       |
| --------------------------------- | --------------------------------- |
| `tar -czf archive.tar.gz dossier` | Compresse un dossier              |
| `tar -xzf archive.tar.gz`         | Décompresse une archive `.tar.gz` |
| `zip archive.zip fichier`         | Crée une archive zip              |
| `unzip archive.zip`               | Décompresse un fichier zip        |
| `gzip fichier`                    | Compresse un fichier              |
| `gunzip fichier.gz`               | Décompresse un fichier `.gz`      |

## Réseau

| Commande                      | Description                          |
| ----------------------------- | ------------------------------------ |
| `ping adresse`                | Teste la connectivité réseau         |
| `curl url`                    | Télécharge ou interagit avec des URL |
| `wget url`                    | Télécharge un fichier                |
| `ifconfig` / `ip a`           | Affiche les interfaces réseau        |
| `netstat -tuln`               | Ports réseau ouverts                 |
| `ssh user@ip`                 | Se connecte en SSH                   |
| `scp fichier user@ip:/chemin` | Copie via SSH                        |

## Redirections et enchaînements

| Syntaxe                  | Description                                 |
| ------------------------ | ------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------- |
| `commande > fichier`     | Redirige la sortie vers un fichier (écrase) |
| `commande >> fichier`    | Ajoute la sortie à la fin du fichier        |
| `commande < fichier`     | Utilise un fichier comme entrée             |
| `commande1               | commande2`                                  | Utilise la sortie de la première comme entrée de la seconde |
| `commande1 && commande2` | Exécute la deuxième si la première réussit  |
| `commande1               |                                             | commande2`                                                  | Exécute la deuxième si la première échoue |
| `commande1 ; commande2`  | Exécute les deux commandes, indépendamment  |

## Commandes avancées et scripts

| Commande            | Description                                       |
| ------------------- | ------------------------------------------------- |
| `echo "texte"`      | Affiche du texte                                  |
| `read variable`     | Lit l’entrée utilisateur dans un script           |
| `#!/bin/bash`       | En-tête d’un script Bash                          |
| `bash script.sh`    | Exécute un script Bash                            |
| `alias ll='ls -l'`  | Crée un alias                                     |
| `source fichier.sh` | Exécute un script dans le shell courant           |
| `cron` / `crontab`  | Planifie des tâches automatiques                  |
| `$?`                | Affiche le code de retour de la dernière commande |

---

```js
console.log("Hello World);
```
