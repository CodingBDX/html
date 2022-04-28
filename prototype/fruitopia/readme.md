# creation fruitopia

## creation navbar
dans vscode pour aller plus vite est creer des multiples elements nous pouvons faire li*3 ainsi il créé 3 elements li

on est pas obligé d'utiliser un space-between entre le logo et le menu `flex:1; text-align:right` permet de marger les elements

pour permettre d'aligner le menu un `display:inline-block` marche et pour enlever les points `list-style:none`

pour creer une petite bar au sjurvol du menu `ul li a::after {
    content: '';
    width: 100%;
    height: 0.4em;
    position: absolute;
    background-color: plum;
    left: 50%;
    transform: translateX(-50%);
    top: -20%;
}`

pour avoir une bar au survol, il faut jouer avec la width `   transition: 0.5s;
}

ul li a:hover::after {
width: 100%;
}`
avec une duration de 0.5s au survol

## flex scinder ecran en 2
un flex sur le parents et sur les 2 enfants un flex-basis:50%;