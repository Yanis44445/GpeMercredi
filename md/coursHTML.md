### Le langage HTML

1. HTML

HyperText Markup Language *Langage de balises hypertexte*

Un fichier `.html` est un fichier de texte (comme le markdown par exemple). On ouvre un fichier de 2 façons:
- le développeur => avec un éditeur de code (ex: VisualStudio Code)
- l'utilisateur => avec un navigateur (ex: firefox)

Le plus souvent les balises html sont en couple (ouvrante/fermante) mais il existe aussi des balises *orpheline*:
- `<MaBalise></MaBalise>`
- `<Mabalise>`

La structure minimale d'une page web est:

```html
<!DOCTYPE html>
<html>  
<head></head>
<body></body>
</html>
```

Le site de référence pour les langages du WEB est le site des développeurs de Mozilla.
[https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements)

Quelques balises à connaître:
- `<body></body>` contient tout ce qui est visible sur la page
- `<head></head>` contient ce qui n'est pas visible sur la page (ex `<title></title>`)
- `<h1></h1>` permet de faire de titres sur la page
- `<p></p>` permet de faire un paragraphe
- `<a href=""></a>` permet d'accrocher le curseur pour cliquer vers un lien
- `<br>` pour casser la ligne
- `<img src="">` pour insérer une image
- `<ul></ul>` pour réaliser une liste sans ordre
- `<ol></ol>` pour réaliser une liste ordonnée
- `<li></li>` pour insérer des items dans une liste


Les balises ouvrantes peuvent contenir des attributs définis sur le site de référence ou l'attribut `class=""`:<br>
`<maBalise attribut=""></maBalise>`

---------------
Pour donner le chemin relatif vers un fichier, on utilise:
- `./` pour chercher dans le dossier courant
- `../` pour chercher dans le dossier du dessus


2. Le CSS
Cascading Style Sheet *feuille de style en cascade*
[https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties)

Pour définir du style, il faut un sélecteur (element HTML ou class), des accolades, une propriété, une valeur.

```css
selecteur{
    propriete:valeur;
}

```

On peut écrire le CSS:
- dans le fichier html entre les balises `<style></style>`
- dans un fichier dédié avec l'extension  `.CSS`  ; il faut ajouter 
une balise `<link rel="stylesheet" href="">`


Il existe plus de 500 prpriétés et encore davantage de valeurs
possibles mais souvent, les valeurs sont : 

- des couleurs (soit un nom soit un code comme rgb(0-255, 0-255, 0-255))
- des tailles: plusieurs unités sont posibles
    -`px` pour pixels
    -`em` relatif à la taille de la police
    -`%` relatif à la taille du contenant 


Rem: Quand le sélécteur css est un élément de même nature, on peut utiliser l'attribut `class` ou `id`. Dans ce cas, le sélécteur est le nom de la classe précédé d'un `.` ou le nom de l'identifiant précédé d'un `#`.

Rem: Le contenu d'un élément html suit le principe du modèle en boîte.
[https://www.w3schools.com/Css/css_boxmodel.asp](https://www.w3schools.com/Css/css_boxmodel.asp)

Trois propriétés importantes sont liées à ce modèle:
-`border` pour le style de la bordure 
-`padding` pour l'espace interne 
-`margin` pour la marge autour de la bordure

Rem: Il existe des propriétés spécifiques au texte, en particulier:
-`text-align` pour justifier le texte
-`font` pour la police de caractères


Ils existent deux balises HTML universelsqui permettent de grouper des éléments ou du texte:
-`<div></div> -<span></span>`