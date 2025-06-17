# 📘 Guide Markdown Complet – Syntaxe de Base

Ce guide présente tous les éléments essentiels pour maîtriser la syntaxe Markdown. Parfait pour créer des README, des documents de cours, des notes de projet ou toute documentation technique.

---

## 🧱 Titres et Hiérarchie

Pour créer des titres, utilisez les symboles `#` suivis d'un espace. Plus il y a de `#`, plus le titre est de niveau inférieur.

```markdown
# Titre niveau 1 (H1)

## Titre niveau 2 (H2)

### Titre niveau 3 (H3)

#### Titre niveau 4 (H4)

##### Titre niveau 5 (H5)

###### Titre niveau 6 (H6)
```

**Rendu :**

# Titre niveau 1 (H1)

## Titre niveau 2 (H2)

### Titre niveau 3 (H3)

#### Titre niveau 4 (H4)

##### Titre niveau 5 (H5)

###### Titre niveau 6 (H6)

---

## ✏️ Formatage du Texte

### Emphases de base

```markdown
**Texte en gras** ou **Texte en gras**
_Texte en italique_ ou _Texte en italique_
**_Texte gras et italique_**
~~Texte barré~~
`Code inline`
```

**Rendu :**

- **Texte en gras**
- _Texte en italique_
- **_Texte gras et italique_**
- ~~Texte barré~~
- `Code inline`

### Autres formatages

```markdown
Texte normal avec du <u>texte souligné</u>
Exposant : H<sup>2</sup>O
Indice : CO<sub>2</sub>
```

---

## 📝 Listes

### Listes à puces non ordonnées

```markdown
- Élément 1
- Élément 2
  - Sous-élément 2.1
  - Sous-élément 2.2
    - Sous-sous-élément 2.2.1
- Élément 3

* Alternative avec astérisque

- Alternative avec plus
```

**Rendu :**

- Élément 1
- Élément 2
  - Sous-élément 2.1
  - Sous-élément 2.2
    - Sous-sous-élément 2.2.1
- Élément 3

### Listes ordonnées

```markdown
1. Premier élément
2. Deuxième élément
   1. Sous-élément numéroté
   2. Autre sous-élément
3. Troisième élément

1) Alternative avec parenthèse
2) Deuxième élément
```

**Rendu :**

1. Premier élément
2. Deuxième élément
   1. Sous-élément numéroté
   2. Autre sous-élément
3. Troisième élément

### Listes de tâches (Todo lists)

```markdown
- [x] Tâche terminée
- [ ] Tâche à faire
- [x] Autre tâche terminée
- [ ] Tâche en cours
  - [x] Sous-tâche terminée
  - [ ] Sous-tâche à faire
```

**Rendu :**

- [x] Tâche terminée
- [ ] Tâche à faire
- [x] Autre tâche terminée
- [ ] Tâche en cours
  - [x] Sous-tâche terminée
  - [ ] Sous-tâche à faire

---

## 🔗 Liens et Images

### Liens

```markdown
[Texte du lien](https://www.exemple.com)
[Lien avec titre](https://www.exemple.com "Titre optionnel")
[Référence vers un titre](#titres-et-hiérarchie)

<!-- Liens de référence -->

[OpenAI][1]
[GitHub][github]

[1]: https://www.openai.com
[github]: https://www.github.com
```

**Rendu :**

- [OpenAI](https://www.openai.com)
- [GitHub avec titre](https://www.github.com "Plateforme de développement")

### Images

```markdown
![Texte alternatif](https://via.placeholder.com/150)
![Image avec titre](https://via.placeholder.com/150 "Titre de l'image")

<!-- Image comme lien -->

[![Image cliquable](https://via.placeholder.com/100)](https://www.google.com)
```

---

## 💬 Citations et Blocs

### Citations

```markdown
> Ceci est une citation simple.

> Ceci est une citation
> sur plusieurs lignes.
>
> Avec un nouveau paragraphe dans la citation.

> ### Citation avec titre
>
> Vous pouvez inclure d'autres éléments Markdown
> dans une citation, comme des **mots en gras**.
```

**Rendu :**

> Ceci est une citation simple.

> Ceci est une citation
> sur plusieurs lignes.
>
> Avec un nouveau paragraphe dans la citation.

### Blocs de code

#### Code inline

```markdown
Utilisez la commande `git status` pour vérifier l'état.
```

#### Blocs de code avec syntaxe

````markdown
```bash
git init
git add .
git commit -m "Initial commit"
git push origin main
```

```python
def saluer(nom):
    return f"Bonjour, {nom}!"

print(saluer("Monde"))
```

```javascript
const saluer = (nom) => {
  return `Bonjour, ${nom}!`;
};

console.log(saluer("Monde"));
```
````

**Rendu :**

```bash
git init
git add .
git commit -m "Initial commit"
git push origin main
```

---

## 📊 Tableaux

### Tableau de base

```markdown
| Colonne 1 | Colonne 2 | Colonne 3 |
| --------- | --------- | --------- |
| Ligne 1   | Données 1 | Info 1    |
| Ligne 2   | Données 2 | Info 2    |
| Ligne 3   | Données 3 | Info 3    |
```

**Rendu :**
| Colonne 1 | Colonne 2 | Colonne 3 |
|--------------|--------------|--------------|
| Ligne 1 | Données 1 | Info 1 |
| Ligne 2 | Données 2 | Info 2 |
| Ligne 3 | Données 3 | Info 3 |

### Tableau avec alignement

```markdown
| Langage    |   Niveau   | Popularité |
| :--------- | :--------: | ---------: |
| HTML       | ⭐⭐⭐⭐☆  | Très haute |
| CSS        | ⭐⭐⭐⭐☆  |      Haute |
| JavaScript |  ⭐⭐⭐☆☆  | Très haute |
| Python     | ⭐⭐⭐⭐⭐ | Très haute |
| Markdown   | ⭐⭐⭐⭐⭐ |      Haute |
```

**Légende alignement :**

- `:---` = Aligné à gauche
- `:---:` = Centré
- `---:` = Aligné à droite

**Rendu :**
| Langage | Niveau | Popularité |
|:-------------|:-----------:|-------------:|
| HTML | ⭐⭐⭐⭐☆ | Très haute |
| CSS | ⭐⭐⭐⭐☆ | Haute |
| JavaScript | ⭐⭐⭐☆☆ | Très haute |
| Python | ⭐⭐⭐⭐⭐ | Très haute |
| Markdown | ⭐⭐⭐⭐⭐ | Haute |

---

## 🔧 Éléments Avancés

### Lignes de séparation

```markdown
---
---

---
```

## **Rendu :**

### Échappement de caractères

```markdown
\*Texte avec astérisques littéraux\*
\# Pas un titre
\[Pas un lien\]
```

**Rendu :** \*Texte avec astérisques littéraux\*

### HTML intégré

```markdown
<details>
<summary>Cliquez pour développer</summary>

Contenu masqué qui s'affiche au clic.

- Liste dans le détail
- Autre élément

</details>

<kbd>Ctrl</kbd> + <kbd>C</kbd> pour copier
```

**Rendu :**

<details>
<summary>Cliquez pour développer</summary>

Contenu masqué qui s'affiche au clic.

- Liste dans le détail
- Autre élément

</details>

### Notes et avertissements

```markdown
> **📝 Note :** Ceci est une information importante à retenir.

> **⚠️ Attention :** Soyez prudent avec cette manipulation.

> **✅ Astuce :** Voici un conseil pratique pour optimiser votre workflow.

> **❌ Erreur :** Évitez cette pratique qui peut causer des problèmes.
```

**Rendu :**

> **📝 Note :** Ceci est une information importante à retenir.

> **⚠️ Attention :** Soyez prudent avec cette manipulation.

---

## 🎯 Conseils et Bonnes Pratiques

### Organisation du document

1. **Utilisez une hiérarchie claire** avec les titres H1, H2, H3...
2. **Ajoutez un sommaire** pour les documents longs
3. **Séparez les sections** avec des lignes horizontales `---`
4. **Utilisez des émojis** pour rendre le contenu plus visuel 🎨

### Formatage du code

- **Code inline** : utilisez les backticks `` ` `` pour les commandes courtes
- **Blocs de code** : spécifiez toujours le langage pour la coloration syntaxique
- **Indentation** : respectez l'indentation pour la lisibilité

### Liens et références

- **Liens externes** : ajoutez des titres descriptifs
- **Liens internes** : référencez les sections de votre document
- **Images** : n'oubliez jamais le texte alternatif

### Listes et tableaux

- **Cohérence** : utilisez le même style de puces dans tout le document
- **Alignement** : alignez correctement les colonnes des tableaux
- **Lisibilité** : évitez les tableaux trop larges

---

## 📚 Ressources Complémentaires

### Outils recommandés

- **Éditeurs** : VS Code, Typora, Mark Text
- **Extensions** : Markdown Preview Enhanced, Markdown All in One
- **Validateurs** : markdownlint, remarklint

### Liens utiles

- [Guide officiel Markdown](https://daringfireball.net/projects/markdown/)
- [GitHub Flavored Markdown](https://github.github.com/gfm/)
- [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

---

## 🎉 Conclusion

Ce guide couvre tous les éléments essentiels de la syntaxe Markdown. Avec ces connaissances, vous pouvez créer des documents professionnels, des README attractifs et une documentation technique claire et structurée.

**Prochaines étapes :**

- [ ] Pratiquer avec un projet personnel
- [ ] Explorer les extensions spécifiques à votre plateforme
- [ ] Créer des templates réutilisables

> **💡 Astuce finale :** La meilleure façon d'apprendre Markdown est de pratiquer régulièrement. Commencez par documenter vos projets !

---
