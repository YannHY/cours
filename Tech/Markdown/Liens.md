# Liens

## Pour mieux comprendre le Markdown

- [Markdown guide](https://www.markdownguide.org/basic-syntax/)
- [Markdown: Basics](https://daringfireball.net/projects/markdown/basics)
- [Markdown Tutorial](https://www.markdowntutorial.com/) (une série de petites leçons et exercices)
- [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)
- [Rédigez en Markdown ! (OpenClassrooms)](https://openclassrooms.com/fr/courses/1304236-redigez-en-markdown)
- [Markdown quick reference cheat sheet](https://wordpress.com/support/markdown-quick-reference/)
- [Using Markdown on WordPress.com](https://wordpress.com/support/can-i-use-markdown-on-wordpress-com/)
- [GitHub Flavored Markdown Spec](https://github.github.com/gfm/)
- [MultiMarkdown](https://fletcherpenney.net/multimarkdown/)

![StackEdit](https://www.ralentirtravaux.com/github/stackedit.png)

## Pour écrire en Markdown

### En ligne

- [StackEdit](https://stackedit.io/)
- [Dillinger](https://dillinger.io/)
- [HackMD](https://hackmd.io/?nav=overview) (son avantage est d’être collaboratif. C’est un peu le Google Docs du Markdown. Il permet aussi de créer des diaporamas.)
- [Dingus](https://daringfireball.net/projects/markdown/dingus)
- [Dillinger](https://dillinger.io/)

### iOS/iPad OS

- [iA Writer](https://apps.apple.com/gb/app/ia-writer/id775737172)
- [Drafts](https://apps.apple.com/gb/app/drafts/id1236254471)
- [Pretext](https://apps.apple.com/gb/app/pretext/id1347707000)
- [Bear](https://apps.apple.com/gb/app/bear/id1016366447)
- [Ulysses](https://apps.apple.com/gb/app/ulysses/id1225571038)
- [Notion](https://apps.apple.com/gb/app/notion-notes-projects-docs/id1232780281)

### Mac

- [Atom](https://atom.io/)
- [Marked 2](https://marked2app.com/)
- [The archive](https://zettelkasten.de/the-archive/)
- [nvALT](https://brettterpstra.com/projects/nvalt/) (voir à propos de cette app [cette introduction](http://aya.io/blog/nvalt-prise-de-notes/))
- [MultiMarkdown Composer](https://multimarkdown.com)

### Multiplateformes

- [Zettlr](https://www.zettlr.com)
- [Typora](https://www.typora.io)

## Réaliser une présentation en Markdown

De la même façon que vous utiliseriez Keynote ou PowerPoint pour réaliser une présentation, vous pouvez utiliser l’une des ressources ci-dessous pour réaliser votre présentation en Markdown.

- [HackMD](https://hackmd.io/?nav=overview) (voir explications ci-dessous)
- [Wunderpresentation](https://wunderpresentation.com) (si vous utilisez [Notion](https://apps.apple.com/gb/app/notion-notes-projects-docs/id1232780281), il vous suffit de copier et coller l’URL et d’appuyer sur `Convertir`. Fonctionne avec d’autres services comme Trello ou Figma).
- [Swipe](https://www.swipe.to)

### Pour mieux comprendre comment utiliser HackMD

- [Make Presentation Slides with HackMD](https://hackmd.io/c/tutorials/%2Fs%2Fhow-to-create-slide-deck)
- [Slide example](https://hackmd.io/slide-example?both)
- [HackMD Tutorial Book](https://hackmd.io/c/tutorials/%2Fs%2Ffeatures#Horizontal-Rules)
- [Features](https://hackmd.io/features?both) (à ouvrir de préférence dans Google Chrome)
- [emoji-cheat-sheet](https://github.com/ikatyang/emoji-cheat-sheet)
- [Font Awesome cheatsheet](https://fontawesome.com/v4.7.0/cheatsheet/) (les icônes de Font Awesome ne marchent dans HackMD qu’avec la version 4.7 ☹️)

## Pourquoi utiliser le Markdown

- [Pourquoi en Markdown ?](https://www.davidbosman.fr/blog/2012/11/23/pourquoi-en-markdown/)
- [My Markdown Writing and Collaboration Workflow, Powered by Working Copy 3.6, iCloud Drive, and GitHub](https://www.macstories.net/ios/my-markdown-writing-and-collaboration-workflow-powered-by-working-copy-3-6-icloud-drive-and-github/)

![Avec Pandoc, convertissez vos fichiers .md](https://www.ralentirtravaux.com/github/pandoc.png)

## Ressources utiles

- [Heck Yes Markdown](http://heckyesmarkdown.com/) (le site convertit n’importe quelle page de votre choix en Markdown)
- [Pandoc](https://pandoc.org/help.html) (pour convertir votre texte en un autre format. Essayez [la version en ligne](https://pandoc.org/try/).)
- [Markdown Table generator](http://www.tablesgenerator.com/markdown_tables) (pour générer automatiquement un tableau)
- [Blot](https://blot.im/) (créer un blog à partir de vos fichiers texte synchronisés avec Dropbox)

### À propos de Pandoc

Avec Pandoc, vous pouvez convertir un fichier avec l’extension .md en fichier .odt. Pour cela, [téléchargez Pandoc](https://pandoc.org/installing.html). Lancez le Terminal. Imaginons que votre fichier se trouve sur le bureau et s’intitule *fichier.md*, tapez `cd ~/desktop` puis `pandoc fichier.md -o fichier.odt`. Et voilà !

Travaillant le plus souvent sur mon iPad, j’apprécie dans [la version en ligne](https://pandoc.org/try/) de pouvoir exporter un texte écrit en Markdown pour le copier dans un wiki sans avoir à faire autre chose qu’appuyer sur conversion. Mais si vous avez votre Mac sous la main ou n’importe quelle app (comme [Screens](https://apps.apple.com/gb/app/screens/id655890150)) vous permettant d’accéder à votre Mac depuis votre iPad, vous pouvez taper la commande `pandoc fichier.md -o fichier.wiki` et voilà !

Si vous avez besoin d’aide à propos de Pandoc, vous pouvez consulter [la documentation](https://pandoc.org/getting-started.html). Il y a également un [groupe de discussion](https://groups.google.com/g/pandoc-discuss) sur Google Groups. 

Si vous avez un Mac et que vous n’aimez pas les lignes de commande, il semble que l’app [MultiMarkdown Converter](https://multimarkdown.com) fasse l’affaire pour une somme relativement modique. Elle repose sur [MMD](https://fletcherpenney.net/multimarkdown/download/) (qui s’utilise justement en ligne de commande)... Mais qui est gratuit...