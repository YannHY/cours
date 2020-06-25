# Écrire des articles pour Vikidia (troisième partie)

## La syntaxe wiki

On parle également de wikicode. Si vous choisissez un article de Vikidia et que vous cliquez sur _[Modifier le wikicode](https://fr.vikidia.org/w/index.php?title=BB-8&action=edit "Modifier le wikicode")_, vous découvrirez le code de la page ou du moins le code du texte affiché dans l'article.

![Afficher le wikicode](https://www.ralentirtravaux.com/github/wikicode.png "Afficher le wikicode")

Qu'est-ce qu'on entend par là ? Pour le dire rapidement, il faut distinguer **la façon dont on écrit un texte** et **la façon dont il s'affiche**. C'est un peu comme le code source d'une page web. Il y a, par exemple, le code HTML et il y a le résultat affiché par le navigateur.

De nombreux utilisateurs sont habitués à des logiciels WYSIWYG (What You See Is What You Get). En d'autres termes, l'action que vous effectuez est immédiatement visible. Par exemple, si vous voulez mettre du texte en gras, vous choisissez de cliquer sur le bouton _Mettre en gras_ (soit en cliquant sur l'icône idoine, soit en allant dans un menu) et le texte sélectionné devient gras.

En HTML ou avec le wikicode, on utilise des signes ou des balises qui vont indiquer qu'il faut afficher le texte en gras. Pour cela, on met des apostrophes au nombre de trois de part et d'autre du mot. Ainsi si vous écrivez `'''BB-8'''`, cela donnera **BB-8**.

Le wikicode est un [langage de balisage](https://fr.wikipedia.org/wiki/Langage_de_balisage "Langage de balisage") léger. Vous en connaissez sûrement d'autres, comme le HTML, le LaTeX, XML, BBCode, Markdown, etc. Ils sont généralement (et pour l'essentiel dont nous avons besoin) très faciles à apprendre.

Si vous n'avez pas bien compris, pas d'inquiétude ! Nous allons reprendre par le menu. Et dans le pire des cas, si vous estimez que c'est trop pour vous, sachez qu'il existe **un éditeur visuel** (un peu comme dans les traitements de texte) qui vous épargne cet apprentissage. Cependant, je trouve que ce serait dommage de ne pas profiter de l'occasion pour sensibiliser les élèves à la notion de code et, par ailleurs, quand on effectue une modification, il est bon de comprendre par quoi elle se traduit dans le code du texte.

Et puis si vraiment vous êtes paralysé à l'idée d'écrire une bêtise, faites-vous la main avec la page du [bac à sable](https://fr.vikidia.org/wiki/Vikidia:Bac_%C3%A0_sable "Bac à sable").

![](https://www.ralentirtravaux.com/github/bacasable.jpeg "Bac à sable")

Cette page est régulièrement remise à zéro par un robot si bien que vous pouvez jouer avec et tenter tout ce que vous voulez, dans les limites de la décence. 😄 Ce sera aussi l'occasion d'indiquer à vos élèves que sur internet, on ne croise pas que des êtres humains mais aussi des robots ! 🤖

Voyons à présent les quelques notions de wikicode dont vous aurez absolument besoin pour écrire votre premier article.

### Le saut de ligne

Si vous souhaitez sauter une ligne, _un seul saut à la ligne_ n'aura aucun effet. Inutile donc de taper sur la touche Retour charriot (la grosse flèche qui fait un angle), cela ne changera rien. Si vous voulez aller à la ligne, il faudra faire _deux sauts à ligne_. Autrement dit, laisser une ligne vide permet de séparer les paragraphes.

Manifestement on peut aussi insérer la balise `<br />`. Une balise est une information comprise entre les signes `<` et `>`. Dans ce cas précis, _br_ signifie _break_. On casse donc la ligne.

Si on écrit cela :

`BB-8 est un personnage de Star Wars.<br />C'est un petit robot.`

On obtiendra cela :

> BB-8 est un personnage de Star Wars.
> 
> C'est un petit robot.

### Mettre un mot en italique

Il faut pour cela simplement mettre 2 apostrophes à gauche et à droite du mot.

Exemple :

`BB-8 est un personnage de Star Wars.<br />C'est un ''petit'' robot.`

Ce qui donne :

> BB-8 est un personnage de Star Wars.
> 
> C'est un _petit_ robot.

### Mettre en gras

On met 3 apostrophes à gauche et à droite du mot :

`'''BB-8''' est un personnage de Star Wars.<br />C'est un ''petit'' robot.`

Et on obtient :

> **BB-8** est un personnage de Star Wars.
> 
> C'est un _petit_ robot.

### Mettre le texte en gras et en italique

Il faut mettre 5 apostrophes à gauche et à droite du mot.

`'''BB-8''' est un personnage de '''''Star Wars'''''.<br />C'est un ''petit'' robot.`

Voici le résultat :

> **BB-8** est un personnage de _**Star Wars**_.
> 
> C'est un _petit_ robot.

#### Récapitulons

`''BB-8''` donne _BB-8_.
`'''BB-8'''` donne **BB-8**.
`'''''BB-8'''''` donne _**BB-8**_.

### Mettre un titre

On met le signe `=` de part et d'autre du titre :

`= Titre principal =`<br />
`== Titre 1 ==`<br />
`=== Titre 2 ===`<br />
`==== Titre 3 ====`

Notez bien que vous n'avez pas besoin de mettre le titre principal. Il est automatiquement généré quand vous créez l'article. Quant aux titres, il faut en comprendre la logique. Les chiffres **n'indiquent pas le numéro du titre** (le premier, le deuxième, le troisième...) mais **leur degré de hiérarchie** dans le texte.

Le titre de niveau 1 (`== Titre 1 ==`) constitue l'une ou plusieurs de vos grandes parties. Il peut donc être utilisé plusieurs fois.

Ainsi, si vous avez un article en trois parties, vous aurez trois titres de niveau 1 :

> == Titre 1 ==<br />
> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi sed cursus ex. Aenean sit amet sem vel nisi iaculis interdum a in risus. Morbi vel gravida eros. Aenean in dignissim ante. In hac habitasse platea dictumst. In viverra purus a enim egestas sollicitudin. Nunc feugiat, velit sed sollicitudin congue, ante elit ultrices justo, nec imperdiet arcu ante sed nibh.
> 
> == Titre 1 ==<br />
> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi sed cursus ex. Aenean sit amet sem vel nisi iaculis interdum a in risus. Morbi vel gravida eros. Aenean in dignissim ante. In hac habitasse platea dictumst. In viverra purus a enim egestas sollicitudin. Nunc feugiat, velit sed sollicitudin congue, ante elit ultrices justo, nec imperdiet arcu ante sed nibh.
> 
> == Titre 1 ==<br />
> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi sed cursus ex. Aenean sit amet sem vel nisi iaculis interdum a in risus. Morbi vel gravida eros. Aenean in dignissim ante. In hac habitasse platea dictumst. In viverra purus a enim egestas sollicitudin. Nunc feugiat, velit sed sollicitudin congue, ante elit ultrices justo, nec imperdiet arcu ante sed nibh.

Si vous avez une sous-partie dans la première partie, alors vous utiliserez pour cela un titre de niveau 2 :

> == Titre 1 ==<br />
> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi sed cursus ex. Aenean sit amet sem vel nisi iaculis interdum a in risus.
> 
> == Titre 2 ==<br />
> Morbi vel gravida eros. Aenean in dignissim ante. In hac habitasse platea dictumst. In viverra purus a enim egestas sollicitudin. Nunc feugiat, velit sed sollicitudin congue, ante elit ultrices justo, nec imperdiet arcu ante sed nibh.
> 
> == Titre 2 ==<br />
> Morbi vel gravida eros. Aenean in dignissim ante. In hac habitasse platea dictumst. In viverra purus a enim egestas sollicitudin. Nunc feugiat, velit sed sollicitudin congue, ante elit ultrices justo, nec imperdiet arcu ante sed nibh.

En somme, le titre principal est le titre de l'article. Le titre 1 est l'une des parties de l'article. Si vous avez besoin d'une sous-partie, utilisez le titre 2. Et si vous voulez mettre une sous-partie dans la sous-partie, choisissez le titre 3 et ainsi de suite.

### Le sommaire

En principe, il n'y a rien à faire. Il se construit automatiquement à partir de trois titres dans l'article.

### Créer une note

Si vous voulez créer des notes de bas de page afin de mettre une référence, utilisez les balises \<ref\> et \</ref\>.

Exemple :

`BB-8 est un personnage de Star Wars<ref>http://www.iphon.fr/post/histoire-robot-bb-8-iphone-839745</ref>.<br />C'est un petit robot.`

> BB-8 est un personnage de Star Wars 1.
> 
> C'est un petit robot.

En bas de page, vous retrouverez l'URL que vous avez mis en note.

### Les liens

Vous serez amenés à créer trois sortes de liens :

- vers un autre article
- vers une image
- vers un lien externe

#### Vers un autre article

Si vous voulez qu'un mot devienne un lien et mène à un autre article de l'encyclopédie Vikidia, placez simplement le mot entre crochets :

`[[Nom de l'article]]`

Si vous souhaitez faire le même lien, mais en affichant un texte différent que celui du nom de l'article, faites ainsi :

`[[Nom de l'article | Titre du lien]]`

#### Vers une image

Pour mettre une image, c'est le même principe, mais il faut faire ainsi :

`[[:Image:Nom de l'image]] `

Remarquez que vous n'avez qu'à mettre le nom de l'image (sans oublier son extension telle que _.jpg_ ou _.png_). Mais pour cela il faut le connaître. Et peut-être même devrez-vous importer l'image (après vous être assuré que vous en aviez les droits).

Pour cela, il faut envoyer votre image sur [Wikimedia Commons](https://commons.wikimedia.org/wiki/Accueil "Wikimedia Commons"). Nous y reviendrons plus loin.

Vous voudrez peut-être aussi indiquer l'emplacement ou la taille de l'image comme ceci :

`[[Fichier:nom de l'image|vignette|droite|Légende de l'image]]`

#### Vers un lien externe

`[[http://adresse.com Titre du lien]]`

### Faire une liste

Vous pouvez avoir besoin de faire deux sortes de listes :

- Les listes non-numérotées (\*)
- Les listes numérotées (\\#)

#### Les listes non-numérotées

Un astérisque permet de faire des listes à puces.

`*Première ligne`<br />
`*Deuxième ligne`<br />
`*Troisième ligne`<br />
`*Quatrième ligne`<br />
`*Cinquième ligne`

Vous pouvez d'ailleurs indenter la liste en ajoutant un deuxième ou troisième astérisque :

`*Première ligne`<br />
`* Deuxième ligne`<br />
`* Troisième ligne`<br />
`**Quatrième ligne`<br />
`**Cinquième ligne`

![Liste à puces créée avec des astérisques](https://www.ralentirtravaux.com/github/liste1.jpeg "Liste à puces créée avec des astérisques")

#### Les listes numérotées

Un dièse (puis deux, puis trois et ainsi de suite) permet de faire des listes numérotées.

`# Première ligne`br />
`# Deuxième ligne`br />
`# Troisième ligne`

Ce qui donne ceci :

> 1. Première ligne
> 2. Deuxième ligne
> 3. Troisième ligne

On a là aussi la possibilité d'indenter en rajoutant un dièse.

![Liste à puces créée avec des dièses](https://www.ralentirtravaux.com/github/liste2.jpeg "Liste à puces créée avec des dièses")

### C'est tout, mais...

Voilà à peu près tout ce dont vous aurez besoin pour écrire un article pour Vikidia. Vous pouvez trouver d'autres explications [sur le site de l'encyclopédie même](https://fr.vikidia.org/wiki/Aide:R%C3%A9sum%C3%A9_de_la_syntaxe_wiki "Syntaxe wiki"). Si d'aventure, il vous prenait l'envie de faire des choses un peu plus complexes, jetez un œil sur [cette page de Wikipédia](https://fr.wikipedia.org/wiki/Aide:Syntaxe_(wikicode) "Wikicode").

Vous y trouverez tout un tas de renseignements. Par exemple, comment insérer un poème (c'est-à-dire avec les balises `<poem>` et donc sans avoir à insérer à chaque fois la balise `<br />`) :

`<poem>`
`Sois sage, ô ma Douleur, et tiens-toi plus tranquille.`
`Tu réclamais le Soir ; il descend ; le voici :`
`Une atmosphère obscure enveloppe la ville,`
`Aux uns portant la paix, aux autres le souci.`
`</poem>`

Vous pourriez également avoir l'idée d'insérer des notes de musique avec la balise `<score>`.

Et entre autres joyeusetés, vous pourriez aussi avoir envie de créer un tableau, ce qui est un véritable casse-tête. Je prends l'exemple de Wikipédia qui propose [sur cette page une aide complète](https://fr.wikipedia.org/wiki/Aide:Ins%C3%A9rer_un_tableau_(wikicode,_avanc%C3%A9) "Insérer un tableau") pour ce qui relève de la syntaxe complexe et qui peut, une fois n'est pas coutume, aussi bien être traitée avec l'assistant visuel. Il vaut d'ailleurs mieux si ni l'anglais ni le HTML ne vous sont familiers.

En tout cas, sachez qu'un tableau ressemble à ça :

` {| class="wikitable alternance center"`
` |+ Titre`
` |-`
` |`
` ! scope="col" | Titre col. A`
` ! scope="col" | Titre col. B`
` ! scope="col" | Titre col. C`
` |-`
` ! scope="row" | Titre ligne 1`
` | Donnée 1A`
` | Donnée 1B`
` | Donnée 1C`
` |-`
` ! scope="row" | Titre ligne 2`
` | Donnée 2A`
` | Donnée 2B`
` | Donnée 2C`
` |-`
` ! scope="row" | Titre ligne 3`
` | Donnée 3A`
` | Donnée 3B`
` | Donnée 3C`
` |}`

Enfin, n'oubliez pas d'indiquer la catégorie à laquelle appartient le travail que vous avez réalisé avec vos élèves en précisant que c'est le fruit d'un travail scolaire. À cet effet, placez ceci qui affichera ce petit rectangle vert :

{{Article fruit d'un travail scolaire}} 

![](https://www.ralentirtravaux.com/github/articlescolaire.jpeg "Article fruit d'un travail scolaire")