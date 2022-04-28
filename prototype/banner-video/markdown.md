# create banner video
pour importer des fonts, il suffit de se rendre sur google font et d'importer avec @import dans le css

les class sont indiquées avec un . et les id avec un # devant les noms

pour focus une class, on indique sa class parent `.parent .child` pour indiquer des parametres au child, il faut l'indiquer dans le parent notemment la taille ou si il sera centrer `justify-content:center`

pour realiser un cercle, il faut appliquer la propriete a une forme carre `border-radius: 50%;`

## javascript
pour appliquer un evenement a une action de l'utilisateur
`document.addEventListener('mousemove')` au mouvement de la souris

    `const dot = document.querySelector('.dot');`

nous attribuons un nom a un selecteur d DOM html la class dot

ensuite nous lui appliquon des paramtres de style
    `dot.style.left = e.pageX + 'px';`

permet d'appliquer un style a gauche dont la function e agit sur le positionnement sur l'axe X


ajoute un listener au click
dot.onclick = function(){}

dans cette function nous voulons lui ajouter une class active


`dot.classList.toggle(active);`

pour prendre en compte se changement il faut que le cursor soit sur le cercle du coup il faut dans le css `transform: translate(50%,50%)` pour bien positionner le curseur

## add text
pour ajouter du text sur cette object mouvent, il faut le faire avec un before ou after .class:before {content: 'text here'};
pour la taille du text font-size:1.5em;

# effect
pour faire un effet d 'halo au click, il faut appliquer cette propriete
`.sec .dot:active {

    box-shadow: 0 0 0 200vh white;
}`
puis dans la class sans active, il faut lui mettre `transition: box-shadow 0.5S` pour controler la durée de l'effet

# text
un text-transform: uppercase permet de mettre toute les lettres en capitale

## video
ajout de la video `    <video autoplay loop muted src="Vegetable stand.mp4"></video>`
il faut ajouter des options autoplay loop et muted si on veut pas le son
puis lui donner une position absolute avec un z-index prioritaire puisque nous avons d'autres position absolute

si vous voulez qu'il soit integrer dans le text, on enleve z-index puis on ajoute dans les lettres
`   mix-blend-mode: multiply;` qui est une sorte d'effet comme photoshop, l'option multiply permet de fusionner comme un calque la video dans le text