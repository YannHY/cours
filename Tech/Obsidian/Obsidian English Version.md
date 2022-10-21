Since I discovered Markdown, several applications have successively seduced me and I first adopted [1Writer](https://1writerapp.com/) and then [Ulysses](https://ulysses.app/) or [Editorial](http://omz-software.com/editorial/). More recently [iA Writer](https://ia.net/fr/writer) and [Bear](https://bear.app/) made me very happy and since I came back to the Mac, I have heard about [Obsidian](https://obsidian.md/).

![[obsidian.png]]

It was love at first sight. Therefore it deserves a separate section [in this little section devoted to Markdown](https://github.com/YannHY/cours/tree/master/Tech/Markdown)). What I would have to say here could be summed up in very few words: do not miss out on such an application. It's a marvel like I haven't seen in 10 years.

However, defining what makes the strength of this app is difficult: a note taking app? A word processing? A [PKM](https://en.wikipedia.org/wiki/Personal_knowledge_management)? Some kind of [IDE](https://en.wikipedia.org/wiki/Integrated_development_environment)? And then explaining what makes Obsidian so rich would take pages and pages, but I can at least give you an idea of its power and show what uses I have developed that were not possible with other applications I have used in the past.

However, there is a good chance that these few weeks spent with Obsidian did not allow me to perceive the entirety of the possibilities which seem immense. Actually, I have the impression of having discovered a new universe, that of PKM (Personal Knowledge Management) actually.

But let's try.

First of all, learn that it all starts with the creation of a “vault”, which is never more than a folder in which you will place all your notes, all your files. You can create several, which I did (one for my lesson plans, one for my reading, one for technology, etc.). In a "vault", you will have an `.obsidian` folder in which will be nestled various things which will be discussed below such as plugins, themes or CSS files.

But let's start with the beginning. Obsidian is above all Markdown.

## 1. Markdown
In a [section dedicated to markdown](https://github.com/YannHY/cours/tree/master/Tech/Markdown), it goes without saying that this is an essential point.

If the importance of keeping control of your data, not entrusting apps that are likely to lock them into an ecosystem that does not care about openness or communication with other applications is an essential feature for you, you will also appreciate that the Markdown remains (more or less) displayed as Markdown and is not subject to any adjustment whatsoever to erase its traces.

Applications that I appreciate a lot like Ulysses, iA Writer or Bear tend to offer their own version of Markdown and take some liberties which I would do well without (and which I do without).

## 2. HTML
Obsidian is based on HTML, JavasScript and CSS. There is even a console like in a browser (`alt + cmd + i`).

![[console.png]]

You therefore have the possibility of inserting HTML. Thus, you can insert various small very useful tags (`<sup> / </sup>`, `<br />` ...), but also, for example, a table (and everyone knows that this is not the strongest point of Markdown). Here's a much more complex one than I could not have done with Markdown alone:

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

But, of course, you can also insert iframes in your notes. This means that you can insert entire web pages, tweets, a list from Dynalist, a Genially, a Google Calendar or even a Pomodoro...

`````
<iframe src="https://pomofocus.io/" height="700" width="700"></iframe>
`````

![[pomodoro.png]]

Maybe it's worth mentioning that I had a problem with displaying tweets. As they are not shown correctly, I have found [Twitframe](https://twitframe.com) which displays a nice and proper tweet.

 ![[tweet.png]]

## 3. CSS Snippets
You can modify the Obsidian style sheet and adapt the display of your notes to your needs. But the stroke of genius is to allow the creation of small "snippets" which replace the modified elements in the main CSS. So you don't have to edit the main file, but can turn on or off certain portions of CSS on the fly.

![[css.png]]

For now, I have contented myself with modifying the appearance of the tags and quotes by copying the code I found here and there. But the next time I want to offer nice documents to my students, I will be able to develop a template of my own.

Anyway, it is quite simple. Just create a `.css` file with your favorite editor. When you are finished, place this file in the snippets folder (`.obsidian> snippets`).

![[css snippets.png]]

Check out the [Meta Post - CSS Themes - Share & showcase - Obsidian Forum](https://forum.obsidian.md/t/meta-post-css-themes/76). You will find pretty things ready to use.

## 4. Themes
Not much to say. The thing is pretty self-explanatory: you can download different "templates". 

Choose the one you like. For my part, I opted for ~~Cybertron~~ Comfort color dark. Go to `Settings> Appearance> Themes`.

![[thèmes.png]]

It is very pleasant to be able to personalize your own working environment. This is, by the way, an area that I have explored very little, but Obsidian's flexibility in this matter is great.

## 5. Links
The ability to link notes together is the first thing that appealed to me when I discovered this kind of apps. I already had this possibility in Bear and since I got a glimpse of the [Zettelkasten](https://zettelkasten.de/) method, this is something that is now essential to me. These are called "wikilinks".

![[liens.gif]]

I use them, among other things, to create a table of contents or to gather scattered notes (for example, all the notes that I take, say, when I read a book by Jules Verne, are thus "connected" a little bit like in a wiki).

![[liens-lecture.png]]

![[table-des-matières.png]]

Just open double square brackets and type the name of the note.

```
[[Note Mysterious Island]]
```

We also have the possibility of aggregating these notes between them. You just have to add an exclamation point, which is handy.

For example, imagine you are a French teacher and you have various scattered texts that you have studied with your students and you want to put them all together to make your exam list. No need to copy and paste everything. Just insert each note into one by inserting the links.

```
! [[Obsidian]]
```

Another interesting possibility: `Copy Obsidian url`. We get something like `obsidian://open? Vault=Tech&file=Markdown%2FObsidian`. That is, if I am not mistaken, some sort of [x-callback-url](http://x-callback-url.com/), which should come in handy for automating some tasks.

Still on the subject of links, in Preview mode, it's quite nice to have this little window for previewing the content of a link, a bit like on Wikipedia, when you hover the mouse over the link.

![[preview.gif]]

## 6. Tags
They are not specific to Obsidian, but I would be sad to do without them. 

As you can see above, with a little CSS, I tried to make them look better. And since I spend time linking my notes together, I also take time to tag everything so that I can better find everything that, in my life as a teacher, I have been able to produce (more on that later). Thus, the tags allow me to carry out a more detailed search to find (for instance) all the writing exercises that I have been able to propose to my students or even sort them by level or subject.

Obviously, this is a work in progress, but just as I want to have documents that are portable regardless of the application I use or will be using, I make sure I can find and gather everything that is still terribly scattered.

Like I said, more on that when it comes to the Dataview plugin.

## 7. Mind map
This is not an essential one but I like the idea of having it: you can export a text file into an image format and thus have a mind map.

![[mindmap.png]]

To get this mind map, open the command (`cmd + P`) and type "mind map". To export the image, click on the three small dots on the right above the mind map and click on "Copy screenshot".

![[mindmap2.png]]

## 8. Graph View
This [Graph View](https://help.obsidian.md/Plugins/Graph+view) is perhaps the prettiest thing I have seen. It is like a starry sky or rather a constellation which allows you to see a graphic representation of your notes. All those that are connected together are linked by a line. Those with the most references are bigger. These dots are all clickable and allow you to navigate easily through this labyrinth made up of your notes. Everything is editable. You can change the CSS. You can filter or only show certain things (orphan notes, images or other documents, etc.). That is wonderful.

![[graph-view.gif]]

## 9. Plugins
Last but not least, plugins.

You will tell me, the "graph view" is a plugin (like the mind map for that matter), but it is a plugin that is part of the "Core plugins". Among these, I also like Tag Pane or Daily Notes. As its name suggests, the latter is used to take daily notes. Basically every time you open the app, a note is created. Convenient for taking notes on the fly. It reminds me a little of [Draft](https://getdrafts.com/) which, each time it is launched, opens a blank page ready to welcome the fruit of your reflections.

There is another set of plugins, third party plugins, made by other developers that bring enrichment to the application that goes beyond expectation.

You will find them by clicking on the small cogwheel at the bottom left corner and then heading to `Community plugins`. You will also need to deactivate the `Safe mode`  (same location).

You can click on any of these links to search for plugins:

- [List of plugins](https://help.obsidian.md/Plugins/List+of+plugins))
- [Third party plugins](https://help.obsidian.md/Advanced+topics/Third-party+plugins)

For now, these are the plugins I use the more:

- [Better Word Count](https://github.com/lukeleppan/better-word-count)
- [Ozan's Image in Editor Plugin](https://github.com/ozntel/oz-image-in-editor-obsidian)
- [Kindle Plugin](https://github.com/hadynz/obsidian-kindle-plugin)
- [Readwise](https://github.com/renehernandez/obsidian-readwise) 
- [Text Snippets](https://github.com/ArianaKhit/text-snippets-obsidian)
- [Pandoc](https://github.com/OliverBalfour/obsidian-pandoc)
- [Review](https://github.com/ryanjamurphy/review-obsidian)
- [Natural language Dates](https://github.com/argenos/nldates-obsidian)
- [Editor Syntax Highlight](https://reposhub.com/javascript/editors/deathau-cm-editor-syntax-highlight-obsidian.html)
- [Advanced Tables](https://github.com/tgrosinger/advanced-tables-obsidian)
- Templates
- [Buttons](https://github.com/shabegom/buttons)
- Tags and Tags pane
- [Dataview](https://github.com/blacksmithgu/obsidian-dataview)

Here is, very quickly, what can be said about these plugins.

### Better Word Count
A very simple plugin that allows you to count the number of words on a page of course (like all counters of this type), but also by selecting a portion of text only. Very handy if you need to fill out a document with a small number of words or if you write your tweets first on Obsidian.

![[word-count.gif]]

### Ozan's Image in Editor Plugin
This plugin allows you to see the images in editor mode while keeping the image link displayed. Note that there is an option in Obsidian that automatically updates this link if you move or rename this link.

![[image.png]]

### Kindle Plugin
Certainly, with the following plugin, the one that made me want to adopt Obsidian.

You can import all the highlighted and annotated excerpts on your Kindle (with [Kindle Highlights](https://read.amazon.com/)). Super handy, because all your quotes are available in text format, so you can easily insert them into an essay or an article. It also allows you to find them more easily perhaps because the search can be filtered using tags.

Do you remember that we can link notes together? You can also link a note to only a part (a block) of another note. Read [Link to blocks](https://help.obsidian.md/How+to/Link+to+blocks) to learn more.

This allows you to insert your quote quite easily.

![[link-block.gif]]

### Readwise
Obviously, I'm not only highlighting things in my Kindle. This is why I use [Readwise](https://readwise.io/) for Kindle Highlights only works with books purchased from Amazon (although you can import the `My Clippings.txt` file from your Kindle), but Readwise also offers to collect pretty much anything you have highlighted and annotated: tweets, saved articles. on Instapaper, Pocket, Books, Feedly, Medium, etc.

![[readwise.png]]

If the topic interests you, take a look at [the Obsidian forum](https://forum.obsidian.md/t/new-plugin-readwise/16006).

### Text Snippets
I have become an absolute fan of this stuff.

François Jourde introduced me to [Text Blaze](https://blaze.today/). I also knew [Text Expander]([Text Expander](https://textexpander.com/)). I use a lot, on the iPad, iPhone or Mac, the Text Replacement function, but this is also available on Obsidian thanks to this plugin.

<iframe border=0 frameborder=0 height=800 width=550   
 src="https://twitframe.com/show?url=https://twitter.com/yannhoury/status/1101188101131653120?ref\_src=twsrc%5Etfw"></iframe>

The idea is to define a keyword (in the example below, the word "I") and when you activate the appropriate keyboard shortcut, it inserts a whole portion of text that has been defined in advance. This is extremely useful when you grade digital essays, for example. 

You define a "snippet" and it inserts the text automatically.

![[snippets.gif]]

### Pandoc
While browsing the export possibilities, I had a feeling of disappointment. 

Only PDF is permitted. Fortunately, a kind developer has created a plugin to take advantage of Pandoc which I have already mentioned [here](https://github.com/YannHY/cours/blob/master/Tech/Markdown/Liens.md#à-propos-de-pandoc).

In short, you install the plugin and to summon Pandoc, run the command (use the shortcut `cmd + P`) then type “Pandoc”.

At first, it didn't work. I had to change the path `/usr/local/bin/pandoc` in settings (after typing `which pandoc` in Terminal). Not sure why, but it works and I can now export to Word, odt, ePub, HTML, etc.

![[pandoc.gif]]

### Natural language Dates & Review
If I write `@Today`, it inserts today's date. Lovely, isn't it?

To be used in combination with Review (`cmd + p`). For example, you select a note or a portion of text, you launch [Review](https://github.com/ryanjamurphy/review-obsidian), choose a date and the selected text will be reminded to you on the given date. I'm not quite sure anymore, but I believe it should be used with the [Calendar](https://github.com/liamcain/obsidian-calendar-plugin) plugin.

![[date.gif]]

### Editor Syntax Highlight
Probably not the plugin that will be the most useful to me, although I gladly use it to store some snippets of code that I use for my website [Ralentir travaux](https://www.ralentirtravaux.com/). But I am thinking above all of my colleagues teaching computer science who will be able to insert portions of code into their courses with syntax highlighting.

![[javascript.png]]

### Advanced table
As you can imagine, this plugin allows you to create tables, which is not the strongest Markdown feature. But, as you can imagine too, this plugin is going to help considerably.

#### How to use it?
I am quoting the explanations found on the developer's [Github account] (https://github.com/tgrosinger/advanced-tables-obsidian).

> To create a table, create a single `|` character, then type the table's first heading and press Tab. Continue entering headings and pressing Tab until all the headings are created. Press Enter to go to the first row. Continue filling cells as before, and press Enter again for each new row.

![[tables.gif]]

When the cursor is placed in the table, you can use the following keyboard shortcuts:

| Hotkey            | Action                      |
| ----------------- | --------------------------- |
| `Tab`             | Next Cell                   |
| `Shift + Tab`     | Previous Cell               |
| `Enter`           | Next Row                    |
| `Cmd + Shift + D` | Open table controls sidebar |

Sometimes the easiest way is still to use the command (`cmd + P`) and type "table" to find what you need.

But that's not all!

#### Formulas
The title is a bit of a spoiler, but you can have formulas in your table as you would with Google Sheets or Excel. Some explanations here:

- [Formulas in Markdown Tables] (https://github.com/tgrosinger/md-advanced-tables/blob/main/docs/formulas.md)
- [Using Excel-like Formulas In Obsidian - Advanced Tables Plugin] (https://www.youtube.com/watch?v=Q0UxmHGoqTk) (a much more practical and faster video to understand how to insert formulas)

Here is what I understood to make a simple addition. At the end of a table,

1. Insert an HTML comment: `<! - ->` (without forgetting the spaces)
2. Add `TBLFM:` (= table format): `<! - TBLFM: ->`
3. Specify the destination & the source (in fact, where the formula will be placed: last row, last column) `@>$2`
4. Specify the formula: `= sum ()`
5. Give the first row: `@I` (= first row under the header)
6. Then the last one: `@-1` (= last row)
7. Use the shortcut (`cmd + option + D`) or the command (` cmd + P`) and choose `evaluate formulas`

You should get this:

```
| Things | Number |
| ------ | ------ |
| One    | 1      |
| Two    | 2      |
| Three  | 3      |
| Total  | 6      |
<!-- TBLFM: @>$2=sum(@I..@-1) -->
```

![[formule.gif]]

I must admit that it is not super user friendly, but it is rather fun (although I will use a spreadsheet preferably for this kind of thing).

 ### Templates
When one wants to avoid writing and rewriting the same thing over and over again, one creates templates.

For example, I created a template to write a lesson plan that I give to my students. The template automatically inserts the main titles and tags.

To do that, I create a new file, use the following shortcut: `cmd + ⇧ + i`, choose the desired template and my lesson plan is automatically inserted. I just have to fill it out.

![[template.gif]]

As a teacher, I would like to use the templates to speed up email writing to communicate more with parents to quickly report any misbehaving or problems.

Anyway, I feel like I'm going to create a lot of templates.
 
If you want to know more, [watch this video made by Bryan Jenks] (https://youtu.be/1eUxQo6Dy7k) to understand how to create templates (the second part of the video talks about the Templater plugin but it seemed a little complex to me).

Also read [Obsidian help] (https://help.obsidian.md/Plugins/Templates). But, basically, it's relatively simple:

1. Activate the templates in Core plugins (in the settings)
2. Create a Templates folder (to store your templates)
3. Create in this folder a template (in fact, a simple file containing everything you want to reuse)
4. Launch your template (for example, you create a file and insert your template into it)

### Buttons
As surprising as it may seem, you can insert a button in a note! Well, after all, we already knew that we could insert an iframe or a table containing a formula like in a spreadsheet. So why not a button? To do this, download the [Buttons] plugin (https://github.com/shabegom/buttons).

There is a wizard for creating a button, but it's actually a few lines of code appearing in your note that contain something like this:

````
```button
name Pin
type command
action Toggle pin
color green
```
^button-buttonpin
````

Basically, you have
- the name of the button (name)
- the type (what the button does)
- the action performed
- the colour

![[button.png]]

OK, but what do we do with that?

Well I imagine the possibilities are quite large (bis repetita ...), but as you will find out in the next section of this article, I created a few on a note that I called the dashboard. In the meantime, know that the options to create the buttons are as follows:

-   **Command:** Click the Button to run a Command from the Command Palette
-   **Link:** Click the Button to open a URL or URI
-   **Calculate:** Click the Button to run a math calculation. Calculate Buttons can reference lines from the note
-   **Template:** Click the Button to prepend, append, insert, or create a new note from a template note
-   **Text:** Clock the Button to prepend, append, insert, or create a new note with specified text
-   **Swap:** A Swap Button is a special type of Inline Button. With a Swap Button you can run a different type of Button on each click

[The best video] (https://youtu.be/2qltHuOjD54) to understand this plugin is from its author (but watch the other two, the developer is funny).

Once the plugin is installed,

1. Run the command `cmd + P`
2. Type "button" (then select "Button Maker")
3. Create your button (select the type of button you want to create from the menu)
4. Change two or three settings (like the appearance or whether you want the button to disappear after it's been used)

You can also choose to insert an "inline button" (the button will be inserted in the line) and it is very elegant.

#### Dashboard
My dashboard is a home page that displays all the tables of content of each folder or sub-folder. By using `![[Text]]`, you can insert the content of a note into another note (remember?). Thus, each table of content can be displayed in the main table and refreshed automatically. Makes sense?

 ![[dashboard.png]]

 The dashboard presents a few buttons (“inline buttons”): Pin, Edit / Preview, New Note, Search ... This allows certain actions to be performed faster. I also placed my tags there or the tasks to be accomplished before 2071.
 
 ### Tags & Tags pane
 First, activate the “Core plugin” Tag pane. As stated in the plugin description:

> Adds a panel on the right that displays all the tags you have, along with their tag count.

And since I found it easier to have it on the left, I simply dragged it to the left to have it next to the magnifying glass or the star where I do my research or place the most frequently used notes. 

About tags ...

I discovered the extent of the possibilities induced by [YAML] (https://youtu.be/rAoFGGMG-0g). To make it very short, YAML = metadata.

As a reminder, metadata is data about your data. It provides information about your data. For example, metadata of a photo give you the size, the type of device, but also the date and time, the location or even, depending on the program you are using, information about people or things appearing in the photo...

The metadata that you are going to place in your notes can therefore be the author, the date, tags and so forth.

To learn more about YAML and how to use it, you can read and see this and that to understand exactly what it's all about:

- [YAML front matter](https://help.obsidian.md/Advanced+topics/YAML+front+matter)
- [YAML | In One Video](https://youtu.be/cdLNKUoMc6c)

Even better, check out [An Introduction to Dataview - Part 1] (https://youtu.be/sEgzrRNkgsE). This is an excellent video for understanding YAML, metadata and above all, as we will see down below, the [Dataview] plugin (https://github.com/blacksmithgu/obsidian-dataview).

YAML data must be placed at the beginning of the file with `---` at the beginning and at the end.

```
---
tags: [Documentation, Markdown]
---
```

Between these `---`, you place a "key" (for example "tags") and a "value" (for example "Markdown"). At the moment Obsidian only accepts three keys: `tags`,` aliases`, and `cssclass`, but that doesn't matter much because you will inevitably be using [Dataview](https: // github. com / blacksmithgu / obsidian-dataview).

The advantages are immense but the first that occurred to me is that my tags do not appear when exporting the note. They don't clutter up the page.

![[yaml.png]]

But above all, we can go much further with [Dataview] (https://github.com/blacksmithgu/obsidian-dataview).

### Dataview
To find out everything that I could not explain to you in a few lines about Dataview, see:

- [An Introduction to Dataview - Part 1](https://youtu.be/sEgzrRNkgsE)
- [An Introduction to Dataview - Part 2](https://youtu.be/jW5pD4SioFM)

It seems, at least if I am to believe those who know exactly what it is, that they look like SQL queries. In fact, you can turn your notes into a database that you can easily extract from.

I can, for example, ask to have a list of all the files located in this folder (providing I click Preview).

Simply write this:

````
```dataview
list
```
`````

But, of course, this is the simplest example I can give.

There is so much more you can do! You can even make tables and sort your notes by date, author or rating, etc.

The best solution is to watch it:

![[dataview-short.gif]]

For that, you will use operators like `from` or `where` to filter the list and display for example a specific hashtag. Or list the contents of a folder (put quotes: `"The folder"`).

You can:
- use boolean operator `AND` or` OR`
- use the minus sign `-Google` to exclude certain terms from the search
- use the `+` sign to concatenate
- create tables
- etc.

## Conclusion
As I said at the beginning of the article, I probably missed a lot of things. I don't really use Hotkeys (not as much as I should) or [Vim](https://www.jamierubin.net/2021/03/23/obsidian-and-vim-mode/). But this permanent feeling of having to discover a vast terra incognita is a real pleasure in the daily use of Obsidian. I know I always have something to explore.

In addition, the application is free. However, I paid £ 25 which gave me access to the beta of the mobile app (which is not in beta anymore by the way). I feel that there is still a lot of work on this side (I would have liked to be able to open files that I share between iA Writer and Working copy). Anyway, I am not paying for the [sync service](https://obsidian.md/sync) since I am using iCloud. On the other hand, I would gladly pay for the [publishing service](https://obsidian.md/publish) (and in fact, I am abandoning the iA / Writer / Working Copy duo).

In my wish list, I would like to find natively the export richness of a Bear or a Draft. Pandoc is awesome, but somewhat insufficient. Maybe I need to master it.

Finally, I would like to see what teachers would do with such an app. It's more of a nerd-oriented use so I'm not sure it appeals to the crowds but who knows.

But what if the students had Obsidian? Imagine the richness of some courses. We would then need a collaborative environment like GitHub. It would be more for high school students, but it could be interesting.

Still, Obsidian can be a bit confusing, if you need more information the following sites have helped me considerably.

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