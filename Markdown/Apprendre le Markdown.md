# Apprendre le Markdown

Le markdown s’apprend en **cinq minutes**. C’est vraiment très simple.

Son intérêt est **triple** :

1. Vous écrivez sur un traitement de texte dont le format est `txt` ou `md`. Autant dire que ce type de fichier sera encore lisible dans 50 ans, quelle que soit l’évolution de l’application que vous utilisez.
2. Vous formatez votre texte sans quitter votre clavier et sans avoir à plonger dans un sous-menu pour obtenir l’effet désiré (ou lorsque les commandes de mise en forme ne sont pas disponibles, comme dans des champs de commentaires de certains sites). 
3. L’export est généralement assez riche : txt, PDF, Docs, HTML, ePub, etc.

## Introduction

> Markdown est un langage de balisage léger créé en 2004 par John Gruber avec l'aide d'Aaron Swartz. Son but est d'offrir une syntaxe facile à lire et à écrire. Un document balisé par Markdown peut être lu en l'état sans donner l’impression d'avoir été balisé ou formaté par des instructions particulières. [Wikipédia](https://fr.wikipedia.org/wiki/Markdown)

Vous connaissez peut-être d’autres langages de balisage comme le HTML ou la syntaxe wiki. Ces « langages » consistent simplement à insérer des balises afin de mettre en forme le texte proposé à la lecture.

Par exemple, en HTML, afin de mettre un mot en gras, on peut utiliser les balises `<b>Mot en gras</b>` pour indiquer que l’on veut que le mot soit affiché en gras. Sur un wiki, on met des apostrophes au nombre de trois de part et d'autre du mot. Ainsi si vous écrivez `'''Mot en gras'''`, cela donnera **Mot en gras**.

Le problème avec certaines balises, c’est que cela rend le texte peu lisible. Or, [comme le dit John Gruber](https://daringfireball.net/projects/markdown/syntax) :

> HTML is a *publishing* format ; Markdown is a *writing* format.

Il s’agit donc d’écrire facilement et lisiblement en vue de publier sur le web (de très nombreuses applications recourent au Markdown : [Wordpress](https://wordpress.com/support/can-i-use-markdown-on-wordpress-com/), [Trello](https://help.trello.com/article/821-using-markdown-in-trello), [Tumblr](https://tumblr.zendesk.com/hc/en-us/articles/231221707-Post-editor), [Day One Journal](http://help.dayoneapp.com/en/articles/440596-markdown-guide), [Discord](https://support.discord.com/hc/en-us/articles/210298617-Markdown-Text-101-Chat-Formatting-Bold-Italic-Underline-), [Bear](https://bear.app/faq/Markup%20:%20Markdown/Markdown%20compatibility%20mode/), etc.)

De fait, si, par exemple, j’écris en HTML « Le [Markdown](https://fr.wikipedia.org/wiki/Markdown), c’est vraiment *pratique* ! », je vais obtenir ceci :

```
<p>Le <a href="https://fr.wikipedia.org/wiki/Markdown" title="Markdown">Markdown</a>, c’est vraiment <em>pratique</em> !</p>
```

Mais en Markdown, cela donnerait ceci :

```
Le [Markdown](https://fr.wikipedia.org/wiki/Markdown), c’est vraiment *pratique* !
```

On remarque que c’est plus épuré, c’est plus lisible en somme et que l’on fait tout en une seule étape. L’écriture et la mise en forme. Votre WordPress — si vous l’utilisez — saura afficher tout ça comme si c’était du HTML. Il y a là un gain de temps appréciable.

## Connaissances de bases à acquérir

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

Rappelons que mettre des titres de cette façon permet de construire dans certains documents la table des matières.

### Mettre en gras, en italique, surligner ou rayer un mot

- Pour mettre un mot en italique, placez ce mot entre deux astérisques `*` : `Ce mot est en *italique*`.
- Pour mettre un mot en gras, places-le entre deux astérisques `**` : `Ce mot est en **gras**`.
- Pour surligner un mot, placez deux signes égal de part et d’autre : `Ce mot est ==surligné==.` 
- Pour barrer un mot, encadrez-le d’un double tilde `~~` : `Ce mot est ~~barré~~`.

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

Si vous voulez faire un lien vers un site externe, simplement mettre le ou les mots entre crochets (j’utilise sur mon iPad le raccourci `⌘ + parenthèse`) suivis du lien mis entre parenthèses, ce qui donne ceci :

```
[Ralentir travaux](https://www.ralentirtravaux.com)
```

C’est facultatif, mais vous pouvez inclure une description du lien dans les parenthèses.

```
[Ralentir travaux](https://www.ralentirtravaux.com "Ralentir travaux, le site du français")
```

Si vous voulez insérer une adresse email, écrivez votre adresse entourée des chevrons `<>`: `<monadresse@truc.com>` .

### Insérer une image

Procédez de la même façon que pour insérer un lien, mais en ajoutant un point d’exclamation avant les crochets. L’URL que vous placerez entre parenthèses sera celle de votre image.

```
![Trois manuels](https://www.ralentirtravaux.com/images/site/trois-manuels.png "Trois manuels")
```

### Insérer un saut de page

Placez trois signes `+++`.

### Insérer une ligne horizontale 

Pour créer une ligne horizontale, insérez trois astérisques (`***`), tiret (`---`) ou « underscores » (`___`) à la suite.

### Citer du texte

Faite précéder le texte d’un simple chevron `>` pour faire une citation 

```
> Sois sage, ô ma Douleur, et tiens-toi plus tranquille.
> Tu réclamais le Soir; il descend; le voici
```

### Faire un tableau

Chaque colonne est séparée d’un pipe (`|` que l’on obtient à l’aide du raccourci `⌘ + ⌥ + L`). Pour faire un rang supplémentaire, allez à la ligne et recommencez.

Voici un exemple :

```
|1re colonne|2e colonne|3e colonne|
|:—|:—:|-:|
|Alignement à gauche|Alignement centré|Alignement à droite|
```

Ce qui donne :

|1re colonne|2e colonne|3e colonne|
|:--|:--:|--:|
|Alignement à gauche|Alignement centré|Alignement à droite|

Vous aurez remarqué que pour aligner le texte à gauche, on insère `:--` dans le deuxième rang. Tandis que pour aligner le texte à droite, on insère `--:`.

## Exemple

Voici un exemple de tableau présentant la conjugaison des temps de l’indicatif.

|Temps simples|Temps composés|
|:--|:--|
|Présent : *je suis*|Passé composé : *j’ai été*|
|Imparfait : *j’étais*|Plus-que-parfait : *j’avais été*|
|Passé simple : *je fus*|Passé antérieur : *j’eus été*|
|Futur simple : *je serai*|Futur antérieur : *j’aurai été*|
|Conditionnel présent : *je serais*|Conditionnel passé : *j’aurais été*|
