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
   
### Les classes pour changer le texte
- text-left
- text-center
- text-right

- text-lowercase
- text-uppercase
- text-capitalize

- font-weight-bold
- font-weight-light
- font-weight-normal
- font-italic

### Les classes pour ajouter l'ombre
- shadow-sm
- shadow
- shadow-lg

### Les classes pour les bordures
````html
<!-- border-top : bordure en haut uniquement -->
<!-- border-secondary : change la couleur de la bordure -->
<footer class="text-muted mt-5 p-3 text-right border-top border-secondary">
   2019 © Chamelles & Co
</footer>
````

### Les bordures arrondies
````html
<!-- rounded : ajoute des bordures arrondies -->
<!-- rounded-circle : ajoute des bordures arrondies pour un carré -->
<!-- rounded-pill : ajoute des bordures arrondies pour un rectangle -->
<div class="bg-danger text-white w-75 p-3 mx-auto rounded">
   Ce site est en construction.
</div>
````

### Rendre les iFrames responsive
````html
<!-- embed-responsive : rend les éléments embarqué (iframe) responsive -->
<!-- embed-responsive-16by9 : Définit la taille d'écran (16:9) -->
<div class="embed-responsive embed-responsive-16by9">
<iframe width="560" height="315" src="https://www.youtube.com/embed/Yomrh4KKQEc" frameborder="0"
allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
allowfullscreen class="embed-responsive-item"></iframe>
<!-- embed-responsive-item : déclare l'objet défini par embed-responsive dans la div parente -->
</div>
````

## Projet 1 : Tinder
Projet permettant de mettre en ouvre toutes les bases apprises sur Bootstrap dans la précédente partie.
### Container
Un containeur sert à englobler l'ensemble du contenu de la page et qui permet les centrer.

## Les composants CSS
### Les boutons

````html
<!-- Crée un bouton rouge -->
<a href="" class="btn btn-danger">Bouton rouge</a>
<!-- Crée un bouton avec un contour rouge -->
<a href="" class="btn btn-outline-danger">Bouton avec contour rouge</a>
<!-- Crée un gros bouton -->
<a href="" class="btn btn-outline-danger btn-lg">Gros bouton</a>
<!-- Crée un petit bouton -->
<a href="" class="btn btn-outline-danger btn-sm">Petit bouton</a>
<!-- Crée un bouton prenant toute la largeur de l'écran -->
<a href="" class="btn btn-outline-danger btn-block">Bouton block</a>
````

### Les messages de succès et d'alertes
````html
<!-- Crée un message d'alerte vert -->
<div class="alert alert-success"> succès </div>
<!-- Crée un message d'alerte avec le lien de la couleur adaptée -->
<div class="alert alert-primary">Alerte avec un <a href="" class="alert-link">lien</a> </div>
<!-- Crée un message d'alerte avec un titre -->
<div class="alert alert-success" role="alert">
  <h4 class="alert-heading">Titre alerte</h4>
  <p>Contenu à afficher.</p>
  <hr>
  <p class="mb-0">Message en plus.</p>
</div>
````

### Les barres de navigation
````html
<!-- navbar : à utiliser pour chaque barre de navigation -->
<!-- bg-light : fond de couleur gris clair -->
<nav class="navbar bg-light">
   <!-- navbar-brand : Nom de la marque -->
   <div class="navbar-brand">Navigation</div>
</nav>
<!-- navbar-dark : barre de navigation à fond noir (transforme le texte en blanc) -->
<!-- bg-dark : fond de couleur noir -->
<nav class="navbar navbar-dark bg-dark">
   <!-- navbar-brand : Nom de la marque -->
   <div class="navbar-brand">Navigation</div>
</nav>
````

### Les badges
````html
<!-- Crée un bouton avec un badge à l'intérieur -->
<div class="btn btn-secondary">
   Messages
   <span class="badge badge-danger">0</span>
</div>
<!-- Badge dans un titre h3 de forme arrondi (ovale) -->
<h3><span class="badge badge-pill badge-danger">Badge</span></h3>
````

### Les formulaires
````html
<section class="p-5 text-center">
   <form>
      <!-- form-group : permet à Bootstrap d'indiquer que le label est lié à l'input -->
      <div class="form-group">
            <label>Prénom</label>
            <!-- input-group : indique ce que l'on veut rajouter à l'input -->
            <div class="input-group">
               <!-- input-group-prepend : indique que l'on veut rajouter quelque chose avant l'élément en question -->
               <div class="input-group-prepend">
                  <div class="input-group-text">@</div>
               </div>
               <!-- form-control : design Bootstrap -->
               <input type="text" name="prenom" placeholder="Saisissez votre prénom" class="form-control">
            </div>
            <!-- Ajoute une description pour l'input -->
            <div class="form-text text-muted">Vous ne pouvez pa mettre de chiffre</div>
      </div>

      <div class="form-group">
            <label>Adresse email</label>
            <!-- readonly : lecture seule, grise l'input -->
            <input type="mail" name="email" value="example@website.fr" readonly placeholder="Saisissez votre prénom"
               class="form-control">
      </div>

      <div class="form-group">
            <label>Adresse email</label>
            <!-- form-control-plaintext : Affichage du texte uniquement sans bordure de l'input -->
            <input type="mail" name="email2" value="example@website.fr" readonly
               placeholder="Saisissez votre prénom" class="form-control-plaintext">
      </div>
   </form>
</section>
````

### Les jumbotrons
Ceux sont des pancartes pour informer les utilisateurs
````html
<!-- A personnaliser à fond -->
<!-- A placer en dehors d'un container -->
<div class="jumbotron">
    <div class="container">
        <!-- display-4 : affichage d'un titre avec texte fin -->
        <div class="display-4">Bienvenue</div>
        <hr>
        <!-- lead : sous-titre -->
        <div class="lead">Ce site parle de Bootstrap</div>
    </div>
</div>
````

### Les cartes
````html
<!-- Création d'une card -->
<div class="card">
   <!-- card-img-top : indique que l'image fait partie de la card (pour garder les dimensions) -->
        <img src="https://static.teteamodeler.com/media/cache/thumb_400/canard-explication-tte-modeler-du-mot-canard.jpeg"
            alt="..." class="card-img-top">
        <div class="card-header">
            Une carte
        </div>
        <div class="card-body">
            <h5 class="card-title">
                Le titre de la carte
            </h5>
            <div class="card-text">
                Le texte qui décrit la carte actuelle
            </div>
        </div>
    </div>
````

### Les barres de progression
````html
<!-- progress : indique que la div contiendra au moins une progress bar -->
<div class="progress mb-2">
   <!-- progress-bar-striped : barre striée -->
   <!-- progress-bar-animated : barre animée -->
   <div class="progress-bar progress-bar-striped progress-bar-animated" style="width: 50%;">50%</div>
</div>

<!-- Addition des barres jusqu'à un max de 100% -->
<div class="progress">
   <div class="progress-bar bg-dark" style="width: 60%;">60%</div>
   <div class="progress-bar bg-success" style="width: 10%;">10%</div>
   <div class="progress-bar bg-warning" style="width: 20%;">20%</div>
</div>
````

### Les breadcrumbs (fil d'ariane)
````html
<ol class="breadcrumb mt-3">
        <li class="breadcrumb-item" aria-current="page"><a href="">Home</a></li>
        <li class="breadcrumb-item active" aria-current="page">Les fils d'ariane</li>
    </ol>
````

## Projet 2 : Site de Tesla
Projet permettant de mettre en ouvre toutes les bases apprises sur Bootstrap dans la précédente partie.

## Les grilles Bootstrap
### La grille
````html
<!-- Création d'une ligne -->
<div class="row">
   <!-- col-{/sm/md/lg/xl}-* -->
   <div class="col-md-6 p-3 bg-dark"></div>
   <div class="col-md-6 p-3 bg-success"></div>
</div>

<div class="row">
   <div class="col p-3 bg-success"></div>
   <div class="col p-3 bg-dark"></div>
</div>
````

### Prioriser des éléments
````html
<div class="row">
   <!-- col-{/sm/md/lg/xl}-* -->
   <!-- order-* : défini l'ordre des div -->
   <div class="col-md-6 p-3 bg-dark order-2"></div>
   <div class="col-md-6 p-3 bg-success order-1"></div>
</div>
````

### Décaler les éléments d'un nombre de colonnes
````html
<!-- Même utilité mais dépécrié -->
    <div class="row mt-3">
        <!-- Donner au offset toujours le même type d'élément (sm,xl...) -->
        <div class="col-sm-4 p-3 bg-success"></div>
        <div class="col-sm-4"></div>
        <div class="col-sm-4 p-3 bg-dark"></div>
    </div>

    <div class="row mt-3">
        <div class="col-sm-3 p-3 bg-success"></div>
        <div class="col-sm-3 p-3 offset-sm-1 bg-secondary"></div>
        <div class="col-sm-3 p-3 offset-sm-1 bg-dark"></div>
    </div>
````

### Aligner verticalement les éléments
````html
<!-- Aligner verticalement des éléments -->
<div class="row mt-1 bg-warning" style="height: 100px">
   <!-- align-self-center : aligne l'item au centre -->
   <div class="col-4 p-3 align-self-center bg-success"></div>
   <!-- align-self-start : aligne l'item en haut -->
   <div class="col-4 p-3 align-self-start bg-secondary"></div>
   <!-- align-self-end : aligne l'item en bas -->
   <div class="col-4 p-3 align-self-end bg-dark"></div>
</div>

<!-- align-items-center : centre tous les éléments de la div -->
<div class="row mt-1 align-items-center bg-warning" style="height: 100px">
   <div class="col-4 p-3 bg-success"></div>
   <div class="col-4 p-3 bg-secondary"></div>
   <div class="col-4 p-3 bg-dark"></div>
</div>
````

### Exercice pratique sur les colonnes (exercice-grille)
Mini exercice pour mettre en oeuvre les éléments appris.

## Les composants d'animation
### Modals
````html
<!-- Bouton d'ouverture du modal -->
<button class="btn btn-primary" data-toggle="modal" data-target="#example">
   Ouvrir
</button>

<!-- Modal -->
<div class="modal" id="example">
   <!-- modal-dialog : Définit tout ce qui va composer la fenêtre -->
   <!-- modal-dialog-centered : centre le modal -->
   <!-- modal-sm (xl) : petit modal -->
   <div class="modal-dialog modal-dialog-centered modal-sm">
      <div class="modal-content">
            <!-- HEADER -->
            <div class="modal-header">
               <h5 class="modal-title">Ma fenêtre</h5>
               <!-- data-dismiss : retire le modal quand le bouton sera utitilisé -->
               <button class="close" data-dismiss="modal">
                  &times;
               </button>
            </div>
            <!-- BODY -->
            <div class="modal-body">
               Le texte de la fenêtre
            </div>
            <!-- FOOTER -->
            <div class="modal-footer">
               <button class="btn btn-secondary" data-dismiss="modal">Fermer</button>
            </div>
      </div>
   </div>
</div>
````

### Carrousels
````html
 <!-- slide : une image -->
    <!-- carousel : plusieurs images qui vont défiler les unes après les autres -->
    <!-- data-ride="carousel" : définit le comportement du carrousel -->
    <div class="carousel slide" data-ride="carousel" id="carouselExample">

        <!-- Indicateurs du carrousel -->
        <ol class="carousel-indicators">
            <li data-target="#carouselExample" data-slide-to="0" class="active"></li>
            <li data-target="#carouselExample" data-slide-to="1"></li>
        </ol>

        <!-- Images du carrousel -->
        <!-- carousel-inner : on rajoute chacun de nos slides à l'intérieur -->
        <div class="carousel-inner">
            <div class="carousel-item active">
                <img src="https://www.dybex.com/modules/ph_simpleblog/covers/2.jpg" alt="Steins;Gate"
                    class="d-block w-100">
                    <!-- Zone de text sur l'image -->
                    <div class="carousel-caption text-dark">
                        <h5>Steins;Gate</h5>
                        <p>Meilleur anime</p>
                    </div>
            </div>
            <div class="carousel-item">
                <img src="https://pm1.narvii.com/6924/2b7439785c11261a878960b44fb295ec0981b3cbr1-1920-1009v2_uhq.jpg"
                    alt="Made in Abyss" class="d-block w-100">
            </div>
        </div>

        <!-- Partie contrôle -->
        <!-- Previous -->
        <a class="carousel-control-prev" data-slide="prev" href="#carouselExample">
            <!-- Définit la forme de la touche previous -->
            <span class="carousel-control-prev-icon"></span>
        </a>
        <!-- Next -->
        <a class="carousel-control-next" data-slide="next" href="#carouselExample">
            <!-- Définit la forme de la touche next -->
            <span class="carousel-control-next-icon"></span>
        </a>
    </div>
````

### Infobulles (au clic)
````html
<!-- data-toggle : Choisi l'animation que l'on souhaite utiliser -->
<!-- data-placement : position d'affichage de l'infobulle -->
<!-- data-content : contenu de l'infobulle -->
<!-- title : titre de l'infobulle -->
<button class="btn btn-primary" data-toggle="popover" data-placement="top"
   data-content="La version bêta n'est pas disponible." title="Information">
   Accéder au site
</button>
<script>
   $(function () {
      $('[data-toggle="popover"]').popover()
   })
</script>
````

### Infobulles (au survol)
````html
<!-- data-toggle : Choisi l'animation que l'on souhaite utiliser -->
<!-- data-placement : position d'affichage de l'infobulle -->
<!-- data-content : contenu de l'infobulle -->
<!-- title : titre de l'infobulle -->
<button class="btn btn-primary" data-toggle="popover" data-placement="top"
   data-content="La version bêta n'est pas disponible." title="Information">
   Accéder au site
</button>
<script>
   $(function () {
      $('[data-toggle="popover"]').popover()
   })
</script>
````

### Les spoilers
````html
<!-- BOUTONS -->
<!-- data-target : id de la cible -->
<button class="btn btn-primary" data-toggle="collapse" data-target="#spoilerA">
   Afficher
</button>

<!-- data-target : pour les boutons -->
<!-- href : pour les liens -->
<a href="#spoilerB" data-toggle="collapse">
   Afficher
</a>

<!-- Ouverture par la classe -->
<button class="btn btn-primary" data-toggle="collapse" data-target=".spoiler-example">
   Afficher
</button>

<!-- SPOILERS -->
<div id="spoilerA" class="collapse spoiler-example">
   <div class="card card-body">
      Le texte du spoiler premier.
   </div>
</div>

<div id="spoilerB" class="collapse spoiler-example">
   <div class="card card-body">
      Le texte du spoiler deuxième.
   </div>
</div>
````

### Boutons avec liste déroulante
````html
<!-- CLASSIQUE -->
<div class="dropdown">
   <!-- BOUTON -->
   <!-- dropdown-toggle : indique que le bouton contient une liste -->
   <button class="btn btn-secondary dropdown-toggle" data-toggle="dropdown">
      Options
   </button>

   <!-- MENU -->
   <div class="dropdown-menu">
      <a class="dropdown-item" href="#">Action</a>
      <a class="dropdown-item" href="#">Action</a>
      <a class="dropdown-item" href="#">Action</a>
   </div>
</div>

<!-- BOUTON + MENU DEROULANT A DROITE -->
<div class="btn-group">
   <!-- BOUTON -->
   <!-- dropdown-toggle : indique que le bouton contient une liste -->
   <button class="btn btn-danger">
      Options
   </button>
   <button class="btn btn-dark dropdown-toggle" data-toggle="dropdown">

   </button>

   <!-- MENU -->
   <div class="dropdown-menu">
      <a class="dropdown-item" href="#">Action</a>
      <a class="dropdown-item" href="#">Action</a>
      <a class="dropdown-item" href="#">Action</a>
   </div>
</div>
````


### Navbar avec menu burger
````html
<!-- navbar-expand-sm : détermine quand la barre passe en menu burger -->
<nav class="navbar navbar-dark navbar-expand-sm bg-dark mt-1">
   <a class="navbar-brand" href="#">Navigation</a>

   <!-- SYSTEME DE SPOILER DANS LA NAVBAR -->
   <button class="navbar-toggler" data-toggle="collapse" data-target="#navbar">
      <span class="navbar-toggler-icon"></span>
   </button>

   <!-- LIENS DE LA NAVBAR -->
   <div class="collapse navbar-collapse" id="navbar">
      <ul class="navbar-nav">
            <li class="nav-item active">
               <a class="nav-link" href="#">Accueil</a>
            </li>
            <li class="nav-item">
               <a class="nav-link" href="#">Lien</a>
            </li>
      </ul>
   </div>
</nav>
````