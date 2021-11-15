# Nomage des sélecteurs HTML

BEM = Bloc Element Modificateur

## BLOC 
 
On nomme un bloc en décrivant sa fonction. 
Nommons notre bloc pour notre aperçu de projet ".proj-prev" 
(prev pour preview ou aperçu en français)
En y assignant uniquement les règles qui sont spécifiques à la configuration de ce bloc en particulier.

/!\ En assignant un paramètre au bloc, tous ses éléments hériteront de ce "paramètre". /!\

Exemple :
```css
.proj-prev {
  color: #fff;
  margin-bottom: .25rem;
}
```

## ELEMENT

Le nom d’un élément doit indiquer deux choses :
- son bloc parent, suivi d’un double underscore (aussi appelé “dunders”) ;
- la fonction de l’élément. Comme c’est le titre de notre projeton va le nommer  ".proj-prev__heading" 
  et lui assigner l’ensemble de règles qui suit.

Exemple :
```css
.proj-prev__heading {
  font-size: 4rem;
  padding-left: 2.5rem;
  margin: 0;
  line-height: 6rem;
}
```

## MODIFICATEUR

Pour cela, vous allez créer un modificateur pour votre bloc ".proj-prev". 
Pour nommer le modificateur, vous devez  : 
- préciser le bloc (ou l’élément) qu’il modifie
- ajouter deux tirets suivi du style graphique de votre modificateur.

Prenons l'exemple de la modification du bloc  ".proj-prev"  pour lui donner un texte vert couleur menthe.
Vous pouvez l’appeler  ".proj-prev--mint"  et lui attribuer une couleur.

Exemple : 
```css
.proj-prev--mint {
  color: #15DEA5;
}
```


## En résumé

BEM signifie bloc, élément, modificateur :
- les blocs sont des bouts de code autonomes ;
- les éléments sont les parties qui forment le bloc ;
- les modificateurs changent l’apparence ou le comportement d’un bloc ou d’un élément.

Les blocs sont nommés en fonction de leur rôle :
- les éléments indiquent le nom de leur bloc parent, suivi d’un double underscore/dunder (__) puis du rôle de l’élément : form__label.

Les modificateurs utilisent le nom du bloc ou de l’élément qu’ils modifient, suivi de deux tirets (--) et de ce que le sélecteur modifie : button--green.

Vous n’avez pas besoin d’attribuer à chaque élément d’une page web un sélecteur de classe.
Vous pouvez utiliser les sélecteurs pour que votre code HTML soit plus propre et concis.
