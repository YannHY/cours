# Apprendre le Markdown

Comme le dit très justement [Wikipédia](https://fr.wikipedia.org/wiki/Markdown),

> Markdown est un langage de balisage léger créé en 2004 par John Gruber avec l'aide d'Aaron Swartz. Son but est d'offrir une syntaxe facile à lire et à écrire. Un document balisé par Markdown peut être lu en l'état sans donner l’impression d'avoir été balisé ou formaté par des instructions particulières.

## Introduction

Vous connaissez peut-être d’autres langages de balisage comme le HTML ou la syntaxe wiki. Ces « langages » consistent simplement à insérer des balises afin de mettre en forme le texte proposé à la lecture.

Par exemple, en HTML, afin de mettre un mot en gras, on peut utiliser les balises `<b>Mot en gras</b>` pour indiquer que l’on veut que le mot soit affiché en gras. Sur un wiki, on met des apostrophes au nombre de trois de part et d'autre du mot. Ainsi si vous écrivez `'''Mot en gras'''`, cela donnera **Mot en gras**.

## Connaissances de bases à acquérir

- Pour mettre un mot en italique, placez ce mot entre deux astérisques `*` : `Ce mot est en *italique*`.
- Pour mettre un mot en gras, places-le entre deux astérisques `**` : `Ce mot est en **gras**`.
- Pour aller à la ligne, appuyez simplement sur la touche `↵`. Si vous souhaitez forcer le retour à la ligne, insérez la balise `<br />`.

## Faire un tableau

### Code

```
|1re colonne|2e colonne|3e colonne|
|:—|:—:|-:|
|Alignement à gauche|Alignement centré|Alignement à droite|
```

### Rendu

|1re colonne|2e colonne|3e colonne|
|:--|:--:|--:|
|Alignement à gauche|Alignement centré|Alignement à droite|

## Exemple

Voici un exemple de tableau présentant la conjugaison des temps de l’indicatif.

|Temps simples|Temps composés|
|:--|:--|
|Présent : *je suis*|Passé composé : *j’ai été*|
|Imparfait : *j’étais*|Plus-que-parfait : *j’avais été*|
|Passé simple : *je fus*|Passé antérieur : *j’eus été*|
|Futur simple : *je serai*|Futur antérieur : *j’aurai été*|
|Conditionnel présent : *je serais*|Conditionnel passé : *j’aurais été*|

## Générer automatiquement un tableau

[Markdown Table generator](http://www.tablesgenerator.com/markdown_tables)