# Pourquoi écrire en Markdown ?

## Une réponse pas si évidente

Il faut bien poser la question puisque la réponse que l’on peut y apporter peut détourner certains de recourir à une telle pratique. Après tout, il est évident que certainement peu de monde a envie d’abandonner son traitement de texte favori. J’imagine que Word a de nombreux fervents. Les utilisateurs de Mac ou d’iPad trouveront dans Pages un joli traitement de texte permettant même de faire des livres numériques. Les fans de Google verront dans Google Docs l’app collaborative par excellence que l’on peut enrichir de merveilleuses extensions.

Alors pourquoi ?

Encore une fois la réponse n’est pas évidente, car je peux imaginer que de nombreux personnes considèrent qu’un logiciel WYSIWYG (What You See Is What You Get) est aujourd’hui la norme et est indispensable. C’est tellement pratique ! On écrit et ce qu’on obtient est absolument similaire à ce qu’on a écrit, et cela séduit immédiatement l’œil quand un traitement de texte recourant au Markdown nécessite un format de sortie. C’est une sorte de code (un format d’entrée) qui nécessitera un format de sortie (de publication si vous préférez). En effet, si vous écrivez en Markdown, ce que vous voyez n’est pas ce que vous aurez : vous écrivez, et votre travail sera ensuite exporté dans l’un des formats de votre choix : rtf, txt, md, docx, PDF, HTML, ePub...

![Le texte écrit en Markdown (Pretext) & lu sur GitHub](https://www.ralentirtravaux.com/github/pretext-github.png)

## Une première réponse

Vous vous direz que vous avez là un premier élément de réponse : **la grande variété de formats possibles**. Mais, pour moi, les premiers éléments de la liste sont les plus importants. En effet, je fuis désormais comme la peste les applications vous enfermant dans un format propriétaire dont la durée de vie peut atteindre un terme prématuré quand une entreprise décide que le logiciel sur lequel vous aviez fondé tous vos espoirs n’est pas financièrement profitable. Par ailleurs, si vous décidez de migrer et qu’un jour vous en avez assez du Mac ou de votre PC, vous envisagerez la portabilité de vos données avec réconfort sinon avec joie. C’est pour cette raison que lorsque je vois des enseignants bâtir leurs séquences entières pour telle ou telle plateforme, je me dis que cela n’est pas prudent. Par exemple si vous créez pendant trois ans des cours pour le TBI Promethean et que vous réalisez (en général bien tardivement) que l’établissement pour lequel vous avez obtenu votre mutation utilise SmartTech, vous allez avoir pas mal de travail de sauvegarde et d’adaptation. Je suis passé par là et la faute incombe aux nombreux logiciels auxquels j’ai confié mes cours : Works, Word, LibreOffice, Pages, Google Docs, etc.

Pour moi, la solution la plus simple est donc alors d’écrire d’abord mes cours sur un traitement de texte comme iA Writer puis d’exporter mon cours dans le format de mon choix (choix fait en fonction de l’établissement dans lequel je me trouve). En l’occurrence, comme nous utilisons massivement la G-Suite, mes cours arrivent sur Google Docs ou au format PDF dans Classroom. Mais je ne veux absolument pas me poser la question du transfert de mes données si un jour (improbable) on abandonne la G-Suite ou si je quitte l’établissement.

Or le format txt ou md autorise cette **portabilité des données**. Par ailleurs le format [texte brut](https://fr.wikipedia.org/wiki/Texte_brut) (*plain text* en anglais) est pérenne. Aucune inquiétude. Il ne dépend pas du bon vouloir d’Apple ou de Microsoft. Le format texte brut est **indestructible**. Ajoutons enfin qu’une application comme [Pandoc](https://pandoc.org/help.html) fait du Markdown un format particulièrement « versatile » et exportable en à peu près tout ce que vous souhaitez (voir, à ce propos, la page [Liens](https://github.com/YannHY/cours/blob/master/Markdown/Liens.md)).

## Les mains sur le clavier

Il y a un autre point qui me plait beaucoup dans le Markdown, c’est la possibilité de **se concentrer sur l’écriture, les deux mains sur le clavier**. J’ai toujours détesté lâcher le clavier, parcourir l’écran pour chercher un menu, puis parfois un sous-menu afin de trouver le réglage nécessaire au formatage du texte. Avec le Markdown, tout est fait au clavier en insérant des balises ou des signes simples : mettre en gras se fait au clavier, créer un lien se fait au clavier, une liste à puces se fait au clavier, etc.

C’est pourquoi j’adore les raccourcis clavier en particulier ceux qui me permettent de me « balader » n’importe où sur la page sans avoir à « caresser » mon trackpad sur des kilomètres.

- Aller du début à la fin de la ligne (et vice versa) : `⌘ + ➝`
- Aller au début ou à la fin d’un mot : `⌥ + ➝`
- Sélectionner lettre par lettre : `⇧ + ➝`
- Sélectionner mot par mot : `⇧ + ⌥ + ➝`
- Sélectionner toute la ligne : `⌘ + ⇧ + ➝` ou sélectionner à partir du curseur du début du texte : `⌘ + ⇧ + ↑` ou vers la fin : `⌘ + ⇧ + ↓` 

## La possibilité d’automatiser

Les traitements de texte reposant sur le Markdown ont une grande flexibilité en ce qui concerne l’automatisation. Si vous êtes arrivé sur cette page, vous avez probablement vu ou lu les articles suivants :

- [Apprendre le Markdown](https://github.com/YannHY/cours/blob/master/Markdown/Apprendre%20le%20Markdown.md)
- [Le guide du Markdown](https://github.com/YannHY/cours/blob/master/Markdown/Le%20guide%20du%20Markdown.md)
- [Markdown et automatisation](https://github.com/YannHY/cours/blob/master/Markdown/Markdown%20et%20automatisation.md)

![Ce script me permet d’écrire avec iA Writer, d’exporter au HTML et de contenir toutes les portions de code nécessaire à l’affichage d’une page sur Ralentir travaux.](https://www.ralentirtravaux.com/github/shortcut.png)

Dans le dernier article, j’évoque Shorcuts sur iOS et iPad OS, mais aussi Automator sur Mac et notamment cette série de scripts :

> Avec les [Markdown Service Tools](https://brettterpstra.com/projects/markdown-service-tools/), vous pouvez choisir certains scripts pour réaliser rapidement différentes manipulations très vite. Ainsi, imaginons que vous souhaitiez sélectionner pour vos élèves une dizaine de sites web dans Safari et constituer une liste contenant le nom du site et le lien afférent. En lançant le script [md - Links - Safari Tabs](https://brettterpstra.com/projects/markdown-service-tools/#linkschrometabssafaritabs) dans TextEdit, vous obtiendrez automatiquement cette liste en un seul clic.

Mais si l’écriture de script n’est pas votre truc (et pour être honnête, ça n’est pas tout à fait le mien), il existe de nombreux services tout prêts à l’emploie précisément comme les susmentionnés Markdown Service Tools, mais aussi des sites qui vous proposent de convertir votre texte en Mardown. Ainsi, je l’ai mentionné plus haut, avec [Pandoc](https://pandoc.org/try/), vous pouvez convertir votre article écrit en Markdown en HTLM 5 pour votre blog ou en Wikicode si vous prévoyez de la partager sur un wiki.

Pour résumer, je trouve que je travaille plus vite depuis que j’utilise le Markdown. Traitement de texte léger, format portable, mains solidement posées sur le clavier, automatisation des tâches... C’est un bonheur d’écrivain (ou d’écrivant en ce qui me concerne).

## Le web sémantique

Il existe une autre raison qui n’est pas spécifiquement inhérente au Markdown, mais qui lui est quand même fortement consubstantielle.

Le Markdown ayant été conçu comme un format de texte pour construire des documents structurés ensuite convertis en HTML, il est, je crois, impossible, d’écrire un texte en Markdown sans que celui n’ait une forte structure qui tient, entre autres, à l’utilisation des titres qui sont hiérarchisés.

Je vous explique. De nombreuses personnes écrivent un document, placent un titre, le mettent en gras et grossissent la police. On pourrait en fait dire que ceci n’est pas un titre. C’est du texte (le corps) qui fait office de titre, mais ce n’est pas un titre. Pas un vrai en tout cas. Même chose avec les sous-titres : un peu de gras, on saute une ligne, etc. Ça ressemble à un sous-titre, mais ça n’en est pas un. Pour que ça en soit, il faudrait aller faire un tour dans les styles et appliquer le style idoine (et c’est bien pratique. C’est même ça qui vous créent de facto une table des matières).

Que ce soit en Markdown ou en HTML, les titres et les sous-titres présentent des différences. Le titre principale est précédé d’un `#` (en Markdown) ou encadré par les balises `<h1></h1>`. Un titre de niveau 2 aura `##` en Markdown ou `<h2></h2>` en HTML, etc. Ça va jusqu’à 6.

Quelle différence ?

Énorme. Un document structuré ainsi est dit sémantique. Il signifie quelque chose — et pas seulement pour le créateur du document —, non, il signifie quelque chose pour le moteur de recherche de Google qui saura indexer correctement votre travail en identifiant le titre principal et ce qui est secondaire ou ce qui se trouve être un paragraphe. Imaginez bien que les machines de Google n’ont aucune idée que l’infâme truc qui trône en haut du document en police 76 de couleur fuchsia est un titre. Seule un document structuré sera en mesure d’être signifiant pour un robot.

Si vous n’êtes pas convaincu, sachez que tout le monde ne « lit » pas le web. Certains l’écoutent et ceux qui ne peuvent alors bénéficier d’un périphérique d’affichage mais recourent à des systèmes auditifs vous seront reconnaissants. La reconnaissance vocale est d’ailleurs ainsi bien meilleure.

En tout cas, tout le monde sera satisfait. Les personnes mal voyantes comme le chercheur qui glanent des informations sur le web.

## Vers un travail collaboratif

Si c’était tout, ce serait déjà pas mal, mais ce serait probablement peu convaincant ou en tout cas pas suffisant pour vous faire adopter le Markdown. Alors, disons-le d’emblée, ce qui me séduit aujourd’hui dans le choix du Markdown est la possibilité de synchroniser mes cours sur GitHub et de rendre mon travail collaboratif.

Pour être tout à fait honnête, la lecture de l’article de MacStories, [My Markdown Writing and Collaboration Workflow, Powered by Working Copy 3.6, iCloud Drive, and GitHub](https://www.macstories.net/ios/my-markdown-writing-and-collaboration-workflow-powered-by-working-copy-3-6-icloud-drive-and-github/), a été pour moi une véritable révélation. J’imagine que j’aurais pu découvrir tout cela plus tôt notamment à travers [cet autre article du même auteur](https://www.macstories.net/stories/one-year-of-ipad-pro/7/). Mais il m’a fallu aussi un peu de temps pour assimiler tout cela.

Reprenons depuis le début.

### La mort de mon disque dur

Je pense que tout a commencé avec la mort de mon disque dur externe ou disons du dernier disque dur que j’ai acheté. Il semble que ces choses-là sont fragiles et j’ai décidé, il y a bien dix ans maintenant au moins, de n’en plus acheter. Jamais. Au lieu de ça, j’ai uploadé (désolé, *téléverser* ne me plait pas) l’ensemble de mes données sur le web. Au début, j’utilisais [iDrive](https://www.idrive.com/) puis j’ai utilisé [Hubic](https://hubic.com/en/) puis iCloud. On ne peut pas dire que ce dernier choix m’ait systématiquement paru satisfaisant tant le cloud d’Apple a pu parfois connaître quelques ratés particulièrement agaçants, mais les choses se sont (un peu) améliorés. 

Bref, depuis, mes données sont en ligne. Je peux quasiment effacer le contenu de mon iPad sans aucun remord. Tout est sauvegardé sans que j’aie à y penser, et je retrouve mes fichiers instantanément si je change de machine.

### Partager, oui. Mais comment ?

Ah ! Mais si tout est en ligne, alors pourquoi ne pas le partager ? Pourquoi ne pas donner le lien du dossier où se nichent mes milliers de fichiers (privilège de vieux) ? Que faire alors ? Donner les droits en écriture ? Cela est risqué. Accorder seulement la lecture seule ? Cela limite la potentielle collaboration. Pendant la pandémie, j’ai pensé partager tous mes cours sur un dossier accessible sur Ralentir travaux. Mais ce n’était pas pratique. Chaque fois que je faisais une modification sur mon traitement de texte, il fallait que j’uploade la nouvelle version en écrasant l’ancienne à l’aide d’un FTP. Fastidieux.

C’est à ce moment que l’article de Federico Viticci m’est revenu en mémoire. Pourquoi ne pas partager mes cours de la façon suivante :

1. Créer un dossier contenant mes cours dans l’application [iA Writer](https://apps.apple.com/gb/app/ia-writer/id775737172).
2. Ouvrir ce même dossier dans Working Copy (un client [GitHub](https://fr.wikipedia.org/wiki/GitHub) pour iPad).
3. Synchroniser ce dossier (un « repository » dans le langage GitHub) sur GitHub (un [« remote »](https://workingcopyapp.com/manual/remotes)).

La plus-value est assez évidente pour qui connait ces applications (j’avoue avoir été assez économe d’explications. Pardonnez-moi. Je vous renvoie aux articles de MacStories qui expliquent tout cela en long et en large).

1. Quoi que j’écrive sur mon traitement de texte favori, les modifications sont automatiquement effectives dans Working Copy. C’est normal puisque les deux apps intègrent le Markdown et exploitent le même dossier. Je n’ai plus ensuite, dans Working Copy, qu’à synchroniser avec GitHub (« commit »).
2. Mes cours sont en ligne. Ils sont sauvegardés. C’est une chose, mais de surcroît, ils peuvent être partagés avec d’autres enseignants. Ceux-ci peuvent proposer des modifications ou suggérer des changements que je suis libre d’accepter ou pas. Et c’est là qu’est l’intérêt de GitHub qui est un service web plutôt orienté développement mais qui est basé un système de contrôle de version. Si bien que si quelqu’un propose une modification, ajoute un paragraphe, enlève un mot, complète avec une phrase, je vais pouvoir très facilement et très agréablement dans une jolie interface comparer les différentes versions du texte et choisir de conserver ou de supprimer tel ou tel ajout.

Au terme de cet article, on peut donc dire que le Markdown est un format simple, pratique, pérenne, flexible, structuré et favorisant la collaboration. Dites ? Vous l’adoptez ?

