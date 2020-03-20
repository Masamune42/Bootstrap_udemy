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

