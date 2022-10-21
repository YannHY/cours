---
tags: [Documentation, Markdown, Obsidian]
---

Depuis que j'ai découvert le Markdown, plusieurs applications m'ont successivement séduit et j'ai tout d'abord adopté  [1Writer](https://1writerapp.com) puis [Ulysses](https://ulysses.app) en passant entre autres par [Editorial](http://omz-software.com/editorial/). Plus récemment [iA Writer](https://ia.net/fr/writer) et [Bear](https://bear.app) ont fait mon bonheur et depuis que je suis un peu revenu au Mac, j'ai entendu parler d'[Obsidian](https://obsidian.md).

![[obsidian.png]]

Le coup de foudre est tel que cela mérite une section à part dans [ce petit dossier consacré au Markdown](https://github.com/YannHY/cours/tree/master/Tech/Markdown). Ce que j'aurais à dire ici pourrait se résumer en très peu de mots : ne passez pas à côté d'une telle application. C'est une merveille comme je n'en ai pas vu depuis 10 ans.

En revanche, définir ce qui fait la force de cette application est difficile (app de prise de notes ? Traitement de texte ? [PKM](https://fr.wikipedia.org/wiki/Gestion_des_connaissances_personnelles) ? Sorte d'[IDE](https://fr.wikipedia.org/wiki/Environnement_de_développement) ?) Et puis expliquer de fond en comble ce qui fait la richesse d'Obsidian prendrait des pages et des pages, mais je peux au moins vous donner une idée de sa puissance et montrer quels sont les usages que j'ai développés et qui n'étaient pas possibles avec les autres applications que j'ai utilisées par le passé.

Il y a toutefois de fortes chances pour que ces quelques semaines passées avec Obsidian ne m'aient pas permis de percevoir l'entiéreté des possibilités qui semblent immenses. C'est à un point tel que j'ai l'impression d'avoir découvert un nouvel univers, celui des PKM (Personal Knowledge Management) en l'occurrence.

Mais enfin essayons.

Tout d'abord, apprenez que tout commence par la création d'un « vault », ce qui n'est jamais qu'un dossier dans lequel vous allez placer toutes vos notes, tous vos fichiers. Vous pouvez en créer plusieurs, ce que j'ai fait (un pour mes cours, un pour mes lectures, etc.). Dans ce « vault », vous aurez un dossier `.obsidian` dans lequel se nicheront différentes choses dont il sera question ci-dessous comme les plugins, les thèmes ou les fichiers CSS.

Mais commençons avec le commencement. Obsidian, c'est avant tout du Markdown.

## 1. Markdown
Dans une [section dédiée au markdown](https://github.com/YannHY/cours/tree/master/Tech/Markdown), il va sans dire que c'est là un point essentiel.

Si l'importance de garder le contrôle de ses données et de ne pas les confier à des apps susceptibles de les enfermer dans un écosystème peu soucieux d'ouverture ou de communication avec d'autres applications est toujours de rigueur, on appréciera aussi que le Markdown reste (à peu près) affiché comme du Markdown et ne fasse pas l'objet d'un aménagement quelconque pour en effacer les traces.

Des applications que j'apprécie beaucoup comme Ulysses, iA Writer ou Bear ont tendance à proposer leur version du Markdown et prennent quelques libertés dont je me passerais bien (et dont je me passe de fait).

## 2. HTML
Obsidian repose sur du HTML, du JavasScript et du CSS. 

On a donc la possibilité d'insérer du HTML. Ainsi, on peut insérer différentes petites balises bien utiles (`<sup>/</sup>`, `<br />`...), mais aussi, par exemple, un tableau (et on sait que ce n'est pas le fort du Markdown). En voici un bien plus complexe que ce que j'aurais pu faire avec le seul Markdown :

````
<table cellpadding="5">
<tr>
<th colspan="2" rowspan="2" style="border-style:none;"></th>
<th colspan = "3">Formes conjointes</th>
<th rowspan="2">Formes<br />disjointes</th>
</tr>
<tr>
<td>Sujet</td>
<td>Complément direct</td>
<td>Complément indirect</td>
</tr>
<tr>
<th rowspan="4">Sing.</th>
<td>1<sup>re</sup> pers.</td>
<td>je</td>
<td>me</td>
<td>me</td>
<td>moi</td>
</tr>
<tr>
<td>2<sup>e</sup> pers.</td>
<td>tu</td>
<td>te</td>
<td>te</td>
<td>toi</td>
</tr>
<tr>
<td>3<sup>e</sup> pers.</td>
<td>il, elle</td>
<td>le, la, en</td>
<td>lui, en, y</td>
<td>lui, elle</td>
</tr>
<tr>
<td></td>
<td></td>
<td>se</td>
<td>se</td>
<td>soi (soi-même)</td>
</tr>
<tr>
<th rowspan="4">Plur.</th>
<td>1<sup>re</sup> pers.</td>
<td>nous</td>
<td>nous</td>
<td>nous</td>
<td>nous</td>
</tr>
<tr>
<td>2<sup>e</sup> pers.</td>
<td>vous</td>
<td>vous</td>
<td>vous</td>
<td>vous</td>
</tr>
<tr>
<td>3<sup>e</sup> pers.</td>
<td>ils, elles</td>
<td>les, leur, se</td>
<td>leur, en, y, se</td>
<td>eux, elles, </td>
</tr>
</table>
````

![[tables.png]]
Mais évidemment, vous pouvez insérer aussi des iframes dans vos notes. Cela veut dire que vous pouvez insérer des pages web entières, des tweets, une liste provenant de Dynalist, un Genially, un Google Calendar voire un Pomodoro...

`````
<iframe src="https://pomofocus.io/" height="700" width="700"></iframe>
`````

![[pomodoro.png]]
Il y a même une console comme dans un navigateur (`alt + cmd + i`).

![[console.png]]
## 3. CSS Snippets
Vous pouvez modifier la feuille de style d'Obsidian et adapter l'affichage de vos textes à vos moindres souhaits. Mais le coup de génie est de permettre de créer de petits « snippets » qui remplacent les éléments modifiés dans le CSS principal. Ainsi, vous n'avez pas à modifier le fichier principal, mais pouvez activer ou désactiver à la volée certaines portions de CSS.

![[css.png]]
Pour l'instant, je me suis contenté de modifier l'apparence des tags et des citations en reprenant le code ici et là. Mais la prochaine fois que je veux proposer des cours à mes élèves, je serai en mesure d'élaborer un template qui m'est propre.

En tout cas, c'est assez simple. Il suffit de créer un fichier `.css` avec votre éditeur préféré. Quand vous avez terminé, placez ce fichier dans le dossier `snippets` (`.obsidian > snippets`).

![[css snippets.png]]
Allez faire un tour sur [Meta Post - CSS Themes - Share & showcase - Obsidian Forum](https://forum.obsidian.md/t/meta-post-css-themes/76). Vous trouvez de jolies choses prêtes à l'emploi.

## 4. Thèmes
Pas grand-chose à dire. La chose est assez explicite en soi : vous pouvez télécharger différents « templates ». Choisissez celui à votre goût. Pour ma part, j'ai opté pour Cybertron. Direction `Settings > Appearance > Themes`.

![[thèmes.png]]
C'est en tout cas bien agréable de pouvoir personnaliser son environnement de travail. C'est, soit dit en passant, un domaine que j'ai bien peu exploré, mais la flexibilité d'Obsidian en la matière est grande.

## 5. Liens
La possibilité de lier des notes entre elles est la première chose qui m'a séduite quand j'ai découvert ce genre d'apps. Je jouissais déjà de cette possibilité dans Bear et depuis que j'ai eu un aperçu de la méthode [Zettelkasten](https://zettelkasten.de), c'est là quelque chose qui m'est désormais essentiel. Ce sont ce qu'on appelle des « wikilinks ».

![[liens.gif]]

Je l'utilise, entre autres, pour créer une table des matières ou pour rassembler des notes éparses (par exemple, toutes les notes que je prends, disons, quand je lis un livre de Jules Verne, sont ainsi « connectées » à la façon d'un lien wiki).

![[liens-lecture.png]]
![[table-des-matières.png]]
Il suffit simplement d'ouvrir de doubles crochets et de taper le nom de la note.

````

[[Note Île mystérieuse]]

````

On a également la possibilité d'agréger ces notes entre elles. Il faut juste ajouter un point d'exclamation, ce qui est bien pratique.

Par exemple, imaginons que vous êtes professeur de français et que vous avez différents textes éparses que vous avez étudiés avec vos élèves et que vous voulez tous les rassembler pour faire votre liste du baccalauréat. Inutile de tout copier coller. Il suffit d'insérer chaque note en une seule en insérant les liens.

````
![[Obsidian]]

````

Autre possibilité intéressante : `Copy Obsidian url`. On obtient quelque chose comme `obsidian://open?vault=Tech&file=Markdown%2FObsidian`. C'est, si je ne m'abuse une sorte de [x-callback-url](http://x-callback-url.com), ce qui devrait s'avérer pratique pour automatiser certaines tâches.

Toujours à propos de lien, en mode Preview, c'est assez agréable d'avoir cette petite fenêtre de prévisualisation du contenu d'un lien, un peu comme sur Wikipédia, quand on passe la souris au-dessus de ce lien.

![[preview.gif]]

## 6.  Tags
Ils ne sont pas spécifiques à Obsidian, mais j'aurais du mal à m'en passer. Comme vous avez pu le voir plus haut, avec un peu de CSS, je me suis efforcé de les rendre plus esthétiques. Et comme je passe du temps à lier mes notes entre elles, je prends aussi du temps pour tout « taguer » afin de pouvoir mieux retrouver tout ce que, dans ma vie d'enseignant, j'ai pu produire. Ainsi, par exemple, les tags me permettent de procéder à une recherche plus fine pour trouver (autre exemple) tous les exercices de rédaction que j'ai pu proposer ou encore les trier par niveau ou sujet.

Évidemment, c'est un travail en cours, mais de la même façon que je tiens à avoir des documents dont la portabilité est assurée quelle que soit l'application que j'utilise ou utiliserai, je veille à pouvoir retrouver et rassembler tout ce qui est encore affreusement éparpillé. Work in progress !

## 7. Mind map
La fonction n'est pas indispensable, mais j'aime bien l'idée de l'avoir : on peut exporter un fichier texte au format image et ainsi avoir une carte mentale.

![[mindmap.png]]
Pour avoir cette carte mentale, ouvrez la commande (`cmd + P`) et tapez « mind map ». Pour exporter l'image, cliquez sur les trois petits points à droite au-dessus de la carte mentale et cliquez sur « Copy screenshot ».

![[mindmap2.png]]
## 8. Graph View
Ce [Graph View](https://help.obsidian.md/Plugins/Graph+view) est peut-être la plus jolie chose que j'ai vue. C'est comme un ciel étoilé ou plutôt une constellation qui donne à voir une réprésentation graphique de vos notes. Toutes celles qui sont liées entre elles sont reliées par un trait. Celles qui ont le plus de références sont plus grosses. Ces points sont tous cliquables et vous permettent de naviguer aisément à travers ce labyrinthe constitué de vos notes. Tout est modifiable. On peut changer le CSS. On peut filtrer ou ne faire apparaitre que certaines choses (les notes orphelines, les images ou autres documents, etc.). C'est merveilleux.

![[graph-view.gif]]

## 9. Plugins
Last but not least, les plugins.

Vous me direz, le « graph view » est un plugin (comme le mind map d'ailleurs), mais c'est un plugin faisant partie des « Core plugins ». Parmi ceux-là, j'affectionne également Daily notes. Comme son nom l'indique, il sert à prendre des notes quotidiennes. En gros, à chaque fois que vous ouvrez l'application, une note est créée. Pratique pour prendre des notes à la volée. Ça me fait un peu penser à [Draft](https://getdrafts.com) qui, à chaque fois qu'on le lance, ouvre une page blanche prête à accueillir le fruit de vos réflexions.

Il existe une autre série de plugins, des plugins de tierce partie qui apportent un enrichissement de l'application qui va au-delà de toute attente.

Vous les trouverez en cliquant sur la petite roue dentée en bas à gauche et en allant dans `Community plugins`. Il vous faudra également désactiver le `Safe mode` (toujours au même endroit).

Vous pouvez cliquer sur l'un de ces liens pour chercher des plugins :

- [Liste des plugins](https://help.obsidian.md/Plugins/List+of+plugins)
- [Plugins de tierce partie](https://help.obsidian.md/Advanced+topics/Third-party+plugins) 

Pour l'instant, j'utilise les plugins suivants :

- [Better Word Count](https://github.com/lukeleppan/better-word-count)
- [Ozan's Image in Editor Plugin](https://github.com/ozntel/oz-image-in-editor-obsidian)
- [Kindle Plugin](https://github.com/hadynz/obsidian-kindle-plugin)
- [Readwise](https://github.com/renehernandez/obsidian-readwise) 
- [Text Snippets](https://github.com/ArianaKhit/text-snippets-obsidian)
- [Pandoc](https://github.com/OliverBalfour/obsidian-pandoc)
- [Review](https://github.com/ryanjamurphy/review-obsidian)
- [Natural language Dates](https://github.com/argenos/nldates-obsidian)
- [Editor Syntax Highlight](https://reposhub.com/javascript/editors/deathau-cm-editor-syntax-highlight-obsidian.html)

Voici, très rapidement, ce que l'on peut dire de ces plugins.

### Better Word Count
Un plugin très simple qui permet de compter le nombre de mots d'une page bien sûr (comme tous les compteurs de ce type), mais aussi en sélectionnant une portion de texte uniquement. Très pratique si vous devez remplir un document avec un nombre de mots réduits ou si vous écrivez vos tweets d'abord sur Obsidian.

![[word-count.gif]]

### Ozan's Image in Editor Plugin
Ce plugin permet de voir les images y compris en mode éditeur tout en gardant cependant l'affichage du lien de l'image. Précisons au passage qu'il y a une option dans Obsidian qui permet de mettre à jour automatiquement ce lien si vous déplacez ou renommez ce lien.

![[image.png]]
### Kindle Plugin
Certainement, avec  le plugin suivant, celui qui m'a donné envie d'adopter Obsidian.

On peut importer tous les extraits surlignés et annotés sur sa Kindle (avec [Kindle Highlights](https://read.amazon.com)). Super pratique, car toutes vos citations sont à votre disposition au format texte et vous pouvez ainsi les insérer facilement dans un essai ou un article. Ça vous permet aussi de les retrouver plus facilement peut-être, la recherche pouvant être filtrée par l'utilisation des tags.

Et vous vous souvenez qu'on peut lier des notes entre elles ? Mais on peut aussi lier une note à une partie seulement (un bloc) d'une autre note (lire [Link to blocks](https://help.obsidian.md/How+to/Link+to+blocks) pour en savoir plus). Un paragraphe par exemple.

Vous pouvez ainsi insérer votre citation assez facilement.

![[link-block.gif]]

### Readwise
Évidemment, il n'y a pas que la Kindle dans la vie. C'est pour ça que j'utilise [Readwise](https://readwise.io/). Kindle Hightlights ne fonctionne qu'avec les livres achetés sur Amazon (encore que vous pouvez importer le fichier `My Clippings.txt` de votre Kindle), mais Readwise propose de collecter à peu près tout ce que vous avez souligné et annoté : tweets, articles sauvegardés sur Instapaper, Pocket, Books, Feedly, Medium, etc.

![[readwise.png]]

Si le sujet vous intéresse, faites un tour sur [le forum](https://forum.obsidian.md/t/new-plugin-readwise/16006).

### Text Snippets
Je suis devenu un fan absolu de ce genre de choses.

François Jourde m'avait fait découvrir [Text Blaze](https://blaze.today). Je connaissais aussi [Text Expander](https://textexpander.com/). J'utilise énormément, sur l'iPad, l'iPhone ou le Mac, la fonction Text Replacement, mais cela est aussi disponible sur Obsidian grâce à ce plugin.

<iframe border=0 frameborder=0 height=800 width=550   
 src="https://twitframe.com/show?url=https://twitter.com/yannhoury/status/1101188101131653120?ref\_src=twsrc%5Etfw"></iframe>

L'idée est de définir un mot-clef (dans l'exemple ci-dessous, le mot « je ») et quand on actionne le racourcci clavier idoine, ça insère toute une portion de texte qu'on a défini à l'avance. C'est extrêmement pratique quand vous corrigez des copies numériques par exemple. Ainsi, au lieu de taper tout le temps :

> Il faut proscrire l’utilisation de la première personne. Il convient de lui préférer un « nous » de modestie ou encore des tournures impersonnelles du type « Il sera question de... », « Il semble que », etc.

Vous définissez un « snippet » et ça insère le texte automatiquement.

![[snippets.gif]]

### Pandoc
En parcourant les possibilités d'export, j'ai eu un sentiment de déception. Seul le PDF est possible de base (comme disent mes filles). Heureusement, un aimable développeur a créé un plugin permettant de tirer partie de Pandoc dont j'ai parlé déjà [en ces lieux](https://github.com/YannHY/cours/blob/master/Tech/Markdown/Liens.md#à-propos-de-pandoc).

Bref, vous installez le plugin et pour convoquer Pandoc, lancez la commande (utilisez le raccourci `cmd + p`) puis tapez « Pandoc ».

Au départ, ça ne marchait pas. J’ai dû changer le chemin `/usr/local/bin/pandoc`  dans les réglages (après avoir tapé `which pandoc`  dans le Terminal). Pas trop sûr d'avoir compris pourquoi, mais ça marche et je peux à présent exporter au format Word, odt, ePub, HTML, etc.

![[pandoc.gif]]

### Natural language Dates & Review
On écrit `@Today` (entre autres) et ça insère la date d'aujourd'hui.

À utiliser combiné avec Review (`cmd + p`). Par exemple, on sélectionne une note ou une portion de texte, on lance [Review](https://github.com/ryanjamurphy/review-obsidian), on choisit une date et le texte sélectionné nous sera rappelé à la date fixée. Je ne suis plus très sûr, mais je crois qu'il faut l'utiliser avec le plugin [Calendar](https://github.com/liamcain/obsidian-calendar-plugin).

![[date.gif]]

### Editor Syntax Highlight
Probablement pas le plugin qui me sera le plus utile, encore que je l'utilise volontiers pour stocker quelques bouts de code que j'utilise pour [Ralentir travaux](https://www.ralentirtravaux.com). Mais je pense surtout à mes collègues de NSI qui vont pouvoir insérer des portions de code dans leurs cours avec la coloration syntaxique.

![[javascript.png]]
## Conclusion
Comme je l'ai dit en début d'article, je suis probablement, forcément passé à côté de beaucoup, beaucoup de choses. Je n'utilise pas vraiment les Hotkeys ni [Vim](https://www.jamierubin.net/2021/03/23/obsidian-and-vim-mode/). Mais cette impression permanente d'avoir à découvrir une vaste terra incognita est un vrai plaisir dans l'utilisation quotidienne d'Obsidian. On sait qu'on a toujours un truc à explorer.

De surcroît, l'application est gratuite. J'ai toutefois payé £25, ce qui m'a donné accès à la bêta de l'app mobile. On sent qu'il y a de ce côté encore pas mal de travail (j'aurais aimé pouvoir ouvrir le dossier que je partage entre iA Writer et Working copy). En tout cas, je ne paye pas pour le [service de synchronisation](https://obsidian.md/sync) puisque j'utilise iCloud. En revanche, je paierais volontiers pour le service de [publication](https://obsidian.md/publish) (et de fait, j'abandonne le couple iA/Writer/Working Copy).

Dans ma wish list, j'aimerais retrouver la richesse d'export d'un Bear ou d'un Draft. Pandoc est appréciable, mais quelque peu insuffisant. Enfin, j'aimerais voir ce que les enseignants feraient avec une telle application. C'est d'un usage plutôt orienté nerd donc je ne suis pas sûr que ça séduise les foules.

Mais si les élèves avaient Obsidian ? Imaginez la richesse de certains cours. Il faudrait alors un environnement collaboratif comme GitHub. Ce serait plutôt pour des lycéens, mais ça pourrait être intéressant.

Reste qu'Obsidian peut un peu dérouter, si vous avez besoin de renseignements supplémentaires, les sites suivants m'ont considérablement aidé.

- [Obsidian Help](https://help.obsidian.md/Index) (-> [Obsidian Mobile](https://help.obsidian.md/Obsidian/Obsidian+Mobile))
- [A Guide to Obsidian: Local, Markdown-Powered Networked Notes](https://www.sitepoint.com/obsidian-beginner-guide/)
- [The Beginner’s Guide to Obsidian Notes Step-by-Step](https://theproductiveengineer.net/the-beginners-guide-to-obsidian-notes-step-by-step/)
- [Your Beginner’s Guide to Obsidian](https://www.keepproductive.com/blog/obsidian-beginners-guide)
- [Playlist (Youtube Channel) about Obsidian](https://www.youtube.com/playlist?list=PLCtt5xdY0d3YAv7pn_6uvp-iaFLpRg_CJ)
- [My top plugins in the Obsidian app](https://youtu.be/X61wRmfZU8Y)
- [Introduction to smart notes with Obsidian and the Zettelkasten Method](https://youtu.be/Etr_Wyfpyvk)
- [The Zettelkasten Method: Examples to help you get started.](https://link.medium.com/dCpWAcIfEgb)
- [Readwise to Obsidian](https://nicolevanderhoeven.com/blog/20210206-readwise-to-obsidian/)
- [Obsidian on Discord](https://discord.com/channels/686053708261228577/694233507500916796)
- [Obsidian on Reddit](https://www.reddit.com/r/ObsidianMD/)
- [How to get fancy with CSS in Obsidian using David Perell’s essays](https://www.youtube.com/watch?v=iCRmtNmGA9k&t=131s) + [Forum Common CSS Hack](https://forum.obsidian.md/t/meta-post-common-css-hacks/1978/13)

https://testflight.apple.com/join/f3moqRS1

[How to install Obsidian on a Chromebook](https://decoge.medium.com/how-to-install-obsidian-on-a-chromebook-53e379217adf)