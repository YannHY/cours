# Apprendre le Markdown

Le markdown s’apprend en **cinq minutes**. C’est vraiment très simple. Son intérêt est **triple** :

1. Vous écrivez sur un traitement de texte dont le format est `txt` ou `md`. Autant dire que ce type de fichier sera encore lisible dans 50 ans quelle que soit l’évolution de l’application que vous utilisez.
2. Vous formatez votre texte sans quitter votre clavier et sans avoir à plonger dans un sous-menu pour obtenir l’effet désiré. 
3. L’export est généralement assez riche : txt, PDF, Docs, HTML, ePub, etc.

## Introduction

Comme le dit [Wikipédia](https://fr.wikipedia.org/wiki/Markdown),

> Markdown est un langage de balisage léger créé en 2004 par John Gruber avec l'aide d'Aaron Swartz. Son but est d'offrir une syntaxe facile à lire et à écrire. Un document balisé par Markdown peut être lu en l'état sans donner l’impression d'avoir été balisé ou formaté par des instructions particulières.

Vous connaissez peut-être d’autres langages de balisage comme le HTML ou la syntaxe wiki. Ces « langages » consistent simplement à insérer des balises afin de mettre en forme le texte proposé à la lecture.

Par exemple, en HTML, afin de mettre un mot en gras, on peut utiliser les balises `<b>Mot en gras</b>` pour indiquer que l’on veut que le mot soit affiché en gras. Sur un wiki, on met des apostrophes au nombre de trois de part et d'autre du mot. Ainsi si vous écrivez `'''Mot en gras'''`, cela donnera **Mot en gras**.

Le problème avec certaines balises, c’est que cela rend le texte peu lisible. Or, [comme le dit John Gruber](https://daringfireball.net/projects/markdown/syntax) :

> HTML is a *publishing* format ; Markdown is a *writing* format.

Il s’agit d’écrire facilement et lisiblement en vue de publier sur le web (de très nombreuses applications recourent au Markdown : Wordpress, Tumblr, Day One Journal, Bear, etc.)

De fait, si, par exemple, j’écris en HTML « Le [Markdown](https://fr.wikipedia.org/wiki/Markdown), c’est vraiment *pratique* ! », je vais obtenir ceci :

```
<p>Le <a href="https://fr.wikipedia.org/wiki/Markdown" title="Markdown">Markdown</a>, c’est vraiment <em>pratique</em> !</p>
```

Mais en Markdown, cela donnerait ceci :

```
Le [Markdown](https://fr.wikipedia.org/wiki/Markdown), c’est vraiment *pratique* !
```

On remarque que c’est plus épuré, c’est plus lisible en somme et que l’on fait tout en une seule étape. L’écriture et la mise en forme. Votre WordPress — si vous l’utilisez — saura afficher tout ça comme si c’était du HTML. Il y a là un gain de temps.

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

### Générer automatiquement un tableau

[Markdown Table generator](http://www.tablesgenerator.com/markdown_tables)