# Créer une page HTML

## La première page

Pour créer la première page de votre site, celle-ci doit être intitulée `index`.

Vous pouvez créer un tel fichier avec un éditeur de texte en général livré avec votre système d’exploitation. Vous pouvez également télécharger un éditeur de texte gratuit offrant l’autocomplétion et la coloration syntaxique rendant l’écriture plus facile et plus rapide.
 
[Brackets](http://brackets.io/) est une application gratuite et open source permettant tout cela.

Votre page `index` doit avoir l’extension `html`. Vous devez donc créer un fichier `index.html`. 

## Structure de votre page

Une page HTML est composée de plusieurs [balises](https://developer.mozilla.org/fr/docs/Apprendre/HTML/Balises_HTML).

La première (qui n’en est pas vraiment une) est une déclaration indiquant simplement que la page est une page HTML écrite en HTML 5 : `<!DOCTYPE html>`.

Elle est d’une grande simplicité. Auparavant, cette déclaration précisait à quelle version du HTML on avait affaire en écrivant quelque chose comme ça :

`<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">`

Aujourd’hui, inutile de préciser quelle version du HTML vous utilisez (bien que l’on sait que ce sera du HTML 5).

Ensuite, il convient d’ouvrir et fermer la balise `<html>`. Votre code HTML sera alors compris entre ces deux balises : `<html></html>`.

On trouve enfin — à l’intérieur des balises `<html>` — deux blocs composés chacun de deux balises : l’une ouvrant et l’autre fermant le bloc. Ces balises sont `<head>` et `<body>`.

On obtient donc

	<!DOCTYPE html>
		<html>
			<head></head>
			<body></body>
		</html>
		
On remarquera deux choses :

1. D’une part, une page HTML est comme un corps humain composé d’une tête (`<head>`) et d’un corps (`<body>`).
2. D’autre part, pour des raisons de clarté, on *indente*, c’est-à-dire qu’on décale le texte à chaque nouveau bloc de balises (comme un alinéa).

L’essentiel de votre code se situera entre les balises `<body></body>`. C’est là que vous allez composer votre page. Ce qui s’affiche d’ailleurs dans votre navigateur doit se situer dans ces balises.

Tout ce qui se trouve entre les balises `<head></head>` ne sera pas affiché sur votre page. Les informations que ces deux balises contiennent peuvent être de nature diverse. On peut mettre, par exemple, les balises `<title></title>` qui donnent un titre à la page, non pas un titre qui sera affiché sur votre page mais plutôt un titre qui s’affichera dans votre navigateur, sur l’onglet par exemple.

On obtient alors

	<!DOCTYPE html>
		<html>
			<head>
				  <title></title>
			</head>
			<body></body>
		</html>

## Les principales balises

Voyons à présent quelques balises vous permettant d’écrire du texte dans votre page. Ces balises devront être comprises entre la balise `<body>` et la balise `</body>`.

### Les titres et les paragraphes

Il existe six différents types de titre tous numérotés de 1 à 6.

	<h1></h1>
	<h2></h2>
	<h3></h3>
	<h4></h4>
	<h5></h5>
	<h6></h6>

Le titre de niveau 1 est le titre principal. C’est le titre qui doit en principe apparaitre en premier et qui donc s’affiche en haut de votre page.

	<h1></h1>

Si votre texte est divisé en deux principales sous-parties, vous recourrez alors aux balises `<h2>` pour le diviser et indiquer les titres des sous-parties.

Si vous souhaitez insérer un paragraphe, placez votre texte entre les balises `<p></p>`.

Voyons un exemple dans lequel nous placerons [une portion de texte ne signifiant pas grand-chose](https://www.lipsum.com/) mais souvent utilisée pour bâtir des exemples de page.

	<!DOCTYPE html>
		<html>
			<head>
				  <title>Lorem ipsum dolor sit amet</title>
			</head>
			<body>
				<h1>Lorem ipsum dolor sit amet</h1>
					<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
				
				<h2>Lorem ipsum dolor sit amet</h2>
					<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
				
				<h2>Lorem ipsum dolor sit amet</h2>
					<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
			</body>
		</html>

Si vous avez besoin de créer un retour à la ligne, il faudra placer la balise `<br/>` (signifiant *break*) et qui permet de *casser* la ligne et donc de créer un retour à la ligne.

	<h1>Lorem ipsum dolor sit amet</h1>
		<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.<br /> Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>

Ainsi après « magna aliqua », il y aura un retour à la ligne.

Précisons une dernière chose. Si vous écrivez en français, les signes diacritiques comme les accents ou les cédilles ne s’afficheront pas correctement. Vous aurez pour cela besoin de placer `<head></head>` une balise dite `meta` (qui peut servir à de nombreux usages) : `<meta charset="UTF-8">`.

Notre première page HTML devrait donc ressembler à ceci :

	<!DOCTYPE html>
		<html>
			<head>
				<meta charset="UTF-8">
				<title>Lorem ipsum dolor sit amet</title>
			</head>
			<body>
				<h1>Lorem ipsum dolor sit amet</h1>
					<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
				
				<h2>Lorem ipsum dolor sit amet</h2>
					<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
				
				<h2>Lorem ipsum dolor sit amet</h2>
					<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
			</body>
		</html>
