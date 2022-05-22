# flexbox

## navbar
display:flex; permet entre autre d'aligner les elements

la propriete list-style: none; permet d'enlever les puces en debut de mot d'une liste

width:max-content; permet d'etendre  les mots d'une liste à la valeur maximal au contraire de min-content qui va contenir les mots ou phrase

la proriete

```css
flex-shrink:0;

```
permet de masquer le menu en flex, on peut scroller à l'horizontale, on peut aussi utiliser la propriete overflow:hidden pour masquer le scroll

```css
gap:1rem;
```
permet de creer des espaces entre les elements comme un margin-right mais il s'applique aux elements qui ont un element

```css
flex-grow:1;
```
flex-grow est interessant il permet que les elements prennent l'ensemble de l'espace

```css
flex-wrap:wrap;
```

tres populaire permet au retrecissement de l'ecran d'aligner les elements dedans, le nowrap permet au element de rester aligner

## flexbox vs grid

.columns > * {  }  permet de selectionner tous les enfants de la div columns

flex-basis:0; garde la meme dimension de la box

si on enleve flex:1; puis la propriete flex-grow:0; le text des box prend le maximum de place
flex-basis a auto, le text des box prend le maximum a l'horizontal

la difference avec width est que flex-basis va inclure les elements dedans (text), du coup l'element sera toujours encadre

## decoration scrollbar
```css 
::-webkit-scrollbar-track {
    background-color: #F5F5F5;
}

::-webkit-scrollbar {
    height: 6px;
    background-color: #F5F5F5;
}

::-webkit-scrollbar-thumb {
    background-color: #3d4852;
    border-radius: 3px;
}

```

permet de changer la couleur,taille des elements d'une scrollbar ou de la faire disparaitre

 overflow-x: scroll; permet d'appliquer un scroll sur les elements

 ```css

  flex-grow: 1;
    flex-shrink: 0;
    flex-basis: 450px;
    margin-left: 1rem;

    ```

    permet de determiner une bonne taille des elements.

    flex-direction indique la direction des div column ou row, utilise dans le @media query


@media (min-width:480px) {
    .cards {
        flex-direction: row;
    }
}

quand il passe au dessus de 480px, il applique une row sur les elements

justify-content est interessant, il centre les elements mais un space-between entre les div avec la même taille d'espacement ou bien positionner par rapport au debut ou la fin de l'element flex-start , flex-end
positionner par exemple un avatar et la date d'écriture d'un article

align-items:flex-start; permet d'adapter la div au positionnement de la plus grande, flex-end place les petites à la fin de la hauteur

## astuce de selection
on peut toujours selectionner des div avec element:ntd-child(numero div){} et on peut changer ce que l'on veut. pour changer sa direction il faut faire un align-self: flex-end; ou flex-stretch

la propriete order:1, permet de donner l'ordre d'apparition avec ntd-child