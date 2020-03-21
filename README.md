# Bootstrap Udemy
BOOTSTRAP 4 : la formation ULTIME
<br>https://www.udemy.com/course/bootstrap-4-la-formation-ultime

## Les bases
### Comment utiliser Bootstrap
2 méthodes : https://getbootstrap.com/
 1. En téléchargeant les fichiers
    - Télécharger un fichier zip contenant des fichiers css et js
    - bootstrap.min.css et bootstrap.min.js à copier / coller
 2. En appelant ceux en ligne
````html
<!-- Dans le head -->
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">

<!-- Avant la fin du body -->
<script src="https://code.jquery.com/jquery-3.4.1.slim.min.js" integrity="sha384-J6qa4849blE2+poT4WnyKhv5vZF5SrPo0iEjwBvKU7imGFAV0wwj1yYfoRSJoZ+n" crossorigin="anonymous"></script>
<script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.0/dist/umd/popper.min.js" integrity="sha384-Q6E9RHvbIyZFJoft+2mJbHaEWldlvI9IOYy5n3zV9zzTtmI3UksdQRVvoxMfooAo" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js" integrity="sha384-wfSDF2E50Y2D1uUdj0O3uMBJnjuUD4Ih7YwaYd1iqfktj0Uod8GCExl3Og8ifwB6" crossorigin="anonymous"></script>
````

### Les classes pour changer la largeur d'un élément
````html
<!-- w-50 : taille de 50% peu importe la taille de l'écran -->
<img src="https://static.wixstatic.com/media/e649e6_70b603238fda46f6be31ee3796577b66~mv2.jpg" class="w-50"/>
<!-- w-auto : taille d'origine peu importe la taille de l'écran -->
<img src="https://static.wixstatic.com/media/e649e6_70b603238fda46f6be31ee3796577b66~mv2.jpg" class="w-auto"/>
````

### Les classes pour changer le fond
````html
<!-- bg-dark : change la couleur du fond en foncé -->
<header class="bg-dark">
   Chamelles & Co
</header>
<!-- bg-danger : change la couleur du fond en rouge -->
<div class="bg-danger">
   Ce site est en construction.
</div>
````

### Les classes pour ajouter des couleurs
Changer la couleur du texte et son opacité.
````html
<!-- text-white : change la couleur du texte en blanc -->
<!-- text-white-50 : change la couleur du texte en blanc avec une opacité de 50 -->
<header class="bg-dark text-white">
   Chamelles & Co
</header>
````

### Ajouter des margin et padding
https://getbootstrap.com/docs/4.4/utilities/spacing/
````html
<!-- p-4 : margin de 4 -->
<!-- Dans la doc Bootstrap : utilisation d'une variable $spacer (SASS), suivant le nombre indiqué, on va multiplié $spacer par un nombre p-3 : *1, p-4 : *1.5 -->
<header class="bg-dark text-white p-4">
   Chamelles & Co
</header>
````

### Exercice
Consignes :
- h1 (marge de 3)
````html
<h1 class="m-3">Bienvenue.</h1>
````
- message d'attention (centré au milieu et padding de 3)
````html
<div class="bg-danger text-white w-75 p-3 mx-auto">
   Ce site est en construction.
</div>
````
- img (marge en haut et en bas de 5 et centré au milieu (utiliser .d-block pour ce faire))
````html
<img src="https://static.wixstatic.com/media/e649e6_70b603238fda46f6be31ee3796577b66~mv2.jpg" class="w-50 my-5 d-block mx-auto" />
````
- h2 (marge de 3)
````html
<h2 class="m-3">Vidéo</h2>
````
- footer (marge en haut de 5 et padding de 3)
````html
<footer class="text-muted mt-5 p-3">
   2019 © Chamelles & Co
</footer>
````

### Les classes pour aligner les éléments
- float
   - float-right
   - float-left
   - float-none

- block / inline
Block : pour avoir un comportement en block, les uns en dessous des autres<br>
Inline : les uns à coté des autres
- d-block
- d-inline
- d-none
````html
<img src="https://static.wixstatic.com/media/e649e6_70b603238fda46f6be31ee3796577b66~mv2.jpg" class="w-50 my-5 d-block mx-auto" />
````

- éléments cachés
   - overflow-auto : barre de défilement ajouté si les éléments sont trop grand par rapport à la zone affichée
   - overflow-hidden : cache la partie des éléments trop grands pour une zone

- les positions
   - position-static : par défaut
   - position-relative : prise en compte de la position par rapport à la balise parente
   - posiition-absolute : par rapport à la page
   - position-fixed : fixe l'élément
   - position-sticky : change la position d'un élément quand il passe sous un élément de la page (pas sur tous les navigateurs)

- Les classes spéciales Bootstrap
   - fixed-top : fixe un élément sur le haut de l'écran
   - fixed-bottom : sur le bas de l'écran (ex : chat Facebook)
   - sticky-top : l'élément reste en position initiale mais si le scroll arrive à l'élément, le laisse en haut de page