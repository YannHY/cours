# Le guide du Markdown

### Faire un paragraphe

Pour aller à la ligne, appuyez simplement sur la touche `↵`. Si vous souhaitez forcer le retour à la ligne, insérez la balise `<br />`.

### Les titres

Comme en HTML, il y a des titres de plusieurs niveaux (1 à 6). On utilise le signe `#` pour ce faire.

```
# Titre de niveau 1
## Titre de niveau 2
### Titre de niveau 3
#### Titre de niveau 4
##### Titre de niveau 5
###### Titre de niveau 6
```

### Mettre en gras ou en italique

- Pour mettre un mot en italique, placez ce mot entre deux astérisques `*` : `Ce mot est en *italique*`.
- Pour mettre un mot en gras, places-le entre deux astérisques `**` : `Ce mot est en **gras**`.

### Insérer une note de bas de page

Placez `[^1]` juste après le mot à la suite duquel vous souhaitez insérez une note de bas de page.

Tout en bas de votre document, insérer alors ceci :

```
[^1]: Ma note de bas de page.
```

### Faire une liste

#### Liste ordonnée

Pour faire une liste ordonnée, simplement numéroter les lignes suivies à chaque fois d’un point :

```
1. Élément 1
2. Élément 2
3. Élément 3
```

#### Liste non-ordonnée

Pour faire une liste non-ordonnée (c’est-à-dire une liste à puces), vous pouvez utiliser au choix le tiret (`-`), l’astérisque (`*`) ou le signe `+`.

```
- Élément 1
- Élément 2
- Élément 3
```

### Mettre un lien

Si vous voulez faire un lien vers un site externe, simplement mettre le ou les mots entre crochets suivis du lien mis entre parenthèses, ce qui donne ceci :

```
[Ralentir travaux](https://www.ralentirtravaux.com)
```

Vous pouvez inclure une description du lien dans les parenthèses.

```
[Ralentir travaux](https://www.ralentirtravaux.com "Ralentir travaux, le site du français")
```

### Insérer une image

Procédez de la même façon que pour insérer un lien, mais en ajoutant un point d’exclamation avant les crochets. L’URL que vous placerez entre parenthèses sera celle de votre image.

```
![Trois manuels](https://www.ralentirtravaux.com/images/site/trois-manuels.png "Trois manuels")
```

### Citer du texte

Faite précéder le texte d’un simple chevron `>` pour faire une citation 

```
> Sois sage, ô ma Douleur, et tiens-toi plus tranquille.
> Tu réclamais le Soir; il descend; le voici
```

### Faire un tableau

Chaque colonne est séparée d’un pipe (`|`). Pour faire un rang supplémentaire, allez à la ligne et recommencez.

Voici un exemple :

```
|1re colonne|2e colonne|3e colonne|
|:—|:—:|-:|
|Alignement à gauche|Alignement centré|Alignement à droite|
```
