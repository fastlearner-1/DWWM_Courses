# 🧠 Git – Commandes essentielles

Ce fichier résume les commandes Git les plus utiles pour la gestion de projets en local et avec un dépôt distant (ex: GitHub).

---

## 🔧 Initialisation et configuration

| Commande                                             | Description                       |
| ---------------------------------------------------- | --------------------------------- |
| `git init`                                           | Initialise un dépôt Git local     |
| `git config --global user.name "Ton Nom"`            | Configure ton nom global          |
| `git config --global user.email "email@example.com"` | Configure ton email global        |
| `git config --list`                                  | Affiche la configuration actuelle |

---

## 📁 Gestion des fichiers

| Commande                  | Description                                             |
| ------------------------- | ------------------------------------------------------- |
| `git status`              | Affiche les fichiers modifiés, en attente ou non suivis |
| `git add fichier.txt`     | Ajoute un fichier à l’index (staging)                   |
| `git add .`               | Ajoute tous les fichiers modifiés                       |
| `git commit -m "Message"` | Valide les modifications avec un message                |
| `git rm fichier.txt`      | Supprime un fichier du projet et de Git                 |
| `git mv ancien nouveau`   | Renomme un fichier suivi par Git                        |

---

## 🔍 Historique et différence

| Commande            | Description                                |
| ------------------- | ------------------------------------------ |
| `git log`           | Affiche l’historique des commits           |
| `git log --oneline` | Historique résumé                          |
| `git diff`          | Affiche les différences entre les fichiers |
| `git show <hash>`   | Détails d’un commit spécifique             |

---

## 🌿 Branches

| Commande            | Description                              |
| ------------------- | ---------------------------------------- |
| `git branch`        | Liste les branches locales               |
| `git branch nom`    | Crée une branche                         |
| `git checkout nom`  | Change de branche                        |
| `git switch nom`    | Change de branche (moderne)              |
| `git merge nom`     | Fusionne une branche dans celle courante |
| `git branch -d nom` | Supprime une branche locale              |

---

## 🌐 Dépôt distant (ex: GitHub)

| Commande                    | Description                                           |
| --------------------------- | ----------------------------------------------------- |
| `git remote add origin URL` | Associe un dépôt distant                              |
| `git push -u origin main`   | Envoie la branche locale `main`                       |
| `git push`                  | Envoie les commits vers le dépôt distant              |
| `git pull`                  | Récupère et fusionne les changements du dépôt distant |
| `git clone URL`             | Clone un dépôt distant en local                       |

---

## 🛠️ Maintenance / réparation

| Commande                      | Description                                   |
| ----------------------------- | --------------------------------------------- |
| `git reset`                   | Réinitialise l’index ou l’historique local    |
| `git checkout -- fichier.txt` | Annule les changements non commités           |
| `git revert <hash>`           | Crée un commit qui annule un commit précédent |
| `git stash`                   | Sauvegarde temporairement les modifs en cours |
| `git stash pop`               | Restaure ce qui a été stashed                 |

---

## 📄 Astuces supplémentaires

- `git commit --amend` : Modifie le dernier commit (contenu ou message)
- `git log --graph --all --oneline` : Affiche un graphe de l’historique
- `git config --global core.editor nano` : Définit un éditeur par défaut
- `.gitignore` : Fichier spécial pour ignorer certains fichiers/dossiers

---

## ✅ Bonnes pratiques

- Commits fréquents et clairs (`git commit -m "Ajout de la fonctionnalité X"`)
- Utilise des branches pour chaque nouvelle fonctionnalité
- Garde `main` propre et stable
- Pousse (`push`) régulièrement vers GitHub

---
