#Slider

Certains vont sans aucun doute se demander : "qu'est-ce qu'un carrousel ?".  Un carrousel, c'est tout simplement un défilement d'images, le plus souvent présent sur l'index d'un site web.

##Objectifs

Vous devez réaliser vous-même un carrousel. Simple dans un premier temps, vous pourrez toujours l'améliorer par la suite si vous êtes motivé ! Ce carrousel, qu'on appellera également slider assez couramment, devra simplement comporter quelques fonctions basiques :
- il devra posséder deux boutons, un pour afficher l'image précédente, l'autre pour afficher la suivante ;
- il saura défiler seul, c'est-à-dire que les images défileront d'elles-mêmes sans que l'on ait à intervenir ;
- il pourra être très flexible dans la mesure où il sera possible de mettre autant d'images que l'on souhaite.

##setTimeout(), ou répéter une fonction régulièrement

Une méthode native de JavaScript va vous être utile pour faire défiler automatiquement les images. Il s'agit de `setTimeout()`, qui prend deux arguments : le nom de la fonction à exécuter, et l'intervalle de temps (en millisecondes) à attendre avant de le faire. L'astuce, c'est de relancer la fonction à l'intérieur d'elle-même pour réaliser une boucle infinie :

```function maBoucle(){
    setTimeout(function(){
        alert('Bonjour !'); // affichera "Bonjour !" toutes les secondes
        maBoucle(); // relance la fonction
    }, 1000);
}

maBoucle(); // on oublie pas de lancer la fonction une première fois```

Les images utilisées ici proviennent de lorempixel.com et ne sont pas toutes libres de droit.

Vous avez maintenant toutes les clés pour réaliser ce carrousel !

N'oubliez pas de consulter la documentation de jQuery si vous en avez besoin, et de faire usage d'un debugger pour localiser un soucis dans votre code.
