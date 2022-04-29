# create site cocacola
pour ma creation des sections, nous mettons un minimum de 100vh pour qu'il prenne l'ensemble de l'ecran a chaque section `min-height:100vh;`

un `justify-content: space-between` pour que les div soit eloigner l'une de l'autre avec un display:flex

un `align-items` pour que ce soit centrer au milieu

## circle
pour que le cercle soit prioritaire, nous lui appliquons une position absolute
ensuite pour le cercle un `clip-path: circle(70% at center center);`

## menu
pour le menu, nous appliquons un header avec une position: absolute ou fixed puis une width:100% pour prendre l'ensemble de l'ecran et une position top et left à 0 avec un petit padding pour ne pas coller les bords
ensuite un justify content: space-between, pour eloigner le logo du menu

un `list-style:none;` est applique pour masquer les puces, et un petit margin left et right entre les noms des categories

sur les liens li a {}, on applique `text-decoration: none;
text-transform: uppercase;
` pour mettre les liens en majuscule et decoration none pour ne plus avoir le text souligne

## conteneur text
sur le text, on applique une position relative avec un max-width de 50% ou 50vw pour que le text ne soit pas sur l'image de droite
pour le paragraph, on change de font `font-family:courrier` puis on espace les lignes `line-height:1.4em`

## bouton
pour appliquer une margin top il faut le declarer en `display:inline-block` ce qui le signal comme un block par rapport au header
text-decoration: none pour enlever le surlignage un petit letter-spacing pour ecarter les lettres entre elles

## social reseaux
nous sortons de la div header, du coup nous mettons en `position:absolute` puis nous indiquons l'emplacement a savoir bottom:1em et left:1em puis nous centrons l'elements
nous lui impliquons un petit effect dessus, `transition: 0.3s ease-in-out
puis sur le hover un transform:translateY pour faire bouger au survol de la souris vers le haut sur l'axe Y

## slide
nous utilisons une bibliotheque js swiper avec un flex-end
`.content .img-box {
    display: flex;
    width: 45vw;
    height: 70vh;
    margin-top: 5em;
    
    justify-content: flex-end;
}`
pour bien le positionner a la fin