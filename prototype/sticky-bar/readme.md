# sticky bar
---
## preview


## sticky with position Y

```css
const nav = document.querySelector('nav')
window.addEventListener('scroll', fixNav)

function fixNav () {
    
    if(window.scrollY > nav.offsetHeight + 150) {
        nav.classList.add('active');
    } else {
        nav.classList.remove('active');
    }
}
```

on va chercher le nav pour indiquer par rapport à la position, on ecoute l'envenement par rapport au scroll.
on indique la condition si la valeur du scroll en Y (vertical) et superieur au nav + 150 (150px) alors on ajoute la class active qui change la couleur de la bar et les liens a

![Alt text](sticky-bar.png?raw=true "Title")