# Blog : avancement du projet  

### Semaine 1:
Au cours de la première semaine du projet, différentes idées ont été explorées. Celles-ci incluent l'observation de la répartition de biens au sein d'un groupe constitué d'altruistes et d'égoïstes, et quel trait de caractère sera majoritaire. De plus, nous avons eu l'idée consistant à examiner comment les stalactites et les stalagmites d'une grotte évoluent en réponse à différentes conditions de température et de lumière a été envisagée.

  

### Semaine 2:
Durant la deuxième semaine,  l'idée d'étudier l'évolution des stalactites et stalagmites d'une grotte en fonction des conditions de température et de lumière a été rejetée. Par la suite, un sujet a été choisi et la problématique formulée : doit-on donner de l'énergie aux autres pays ? La pertinence du sujet a été évaluée. Les règles de modélisation ont commencé à être établies. Les conditions prises en compte incluent uniquement la production et la consommation d'énergie, les ressources, le prix de l'échange, la limite de tour non-stable avant fusion, et le pourcentage d'énergie donnée lors des échanges. Les contextes géopolitiques ou dynamiques de pouvoir n'ont pas été pris en compte pour faciliter l'implémentation de variables qui ont été choisi dans l'objectif de simplifier au plus le modèle sans en retirer la complexité nécessaire.

  

### Semaine 3:
Cette troisième semaine a été consacrée à la mise en place des premières fonctions et des classe pouvant représenter le modèle, notament la classe Pays, que l'on peut généraliser comme étant une unité de groupe,  ainsi qu'à la recherche documentaire. Des difficultés ont été rencontrées pour trouver du contenu relatif à des sujets similaires sans être hors sujet car les sources truvées s'orientent trop souvent sur des sujets purement d'économie, ou purement mathématique.

  

### Semaine 4:
Au cours de la quatrième semaine, le code a été continué. L'implémentation de la visualisation via l'interface pygame a été réalisée. Les fonctions suivantes ont été mises en place : une fonction qui échange l'énergie contre des ressources entre deux pays, une fonction qui vérifie la stabilité d'un pays, une fonction qui génère un pays aléatoire, une fonction qui génère une grille remplie de pays aléatoires, une fonction qui renvoie une grille avec la stabilité des pays, une fonction qui renvoie le pourcentage de pays stables dans une grille, et enfin une fonction qui renvoie le voisinage d'un pays.

  

### Semaine 5:
Cette cinquième semaine a été consacrée à l'utilisation du théorème des quatre couleurs sur l'interface pygame pour s'assurer que tous les pays limitrophes sont de couleurs différentes. Ainsi, il est possible de faire la distinction entre deux pays collés l'un à l'autre dans le cas où un pays fusionne avec un autre et prend donc plus d'une case.

  

### Semaine 6:
Au cours de la sixième semaine, le code a été continué avec l'implémentation de la fonction de fusion des pays, qui s'avère être en réalité l'alliance de deux pays pour effectuer des échanges. De la découle la notion de dépendance d'un pays envers l'autre. Quelques détails de l'interface pygame ont été amélioré, avec de la surbrillance sur les cases et lorsque l'on clique sur une case elle s'assombrie et cela affiche les informations du pays et ce jusqu'à ce qu'on clique sur un autre pays.

  

### Semaine 7:
La septième semaine a été consacrée à la finalisation du menu avec des entrées et sorties de données. Si aucune entrée n'est donnée, des valeurs aléatoires sont générées. Le carnet de bord des recherches documentaires a également été finalisé.

  

### Semaine 8:
Pendant la huitième et dernière semaine la logique d'itération pour le code a été finalisée. Toute la logique et les fonctions logiques ont été implémentées dans l'affichage. Le tout s'affiche à peu près normalement, mais il y avait encore un problème avec les pays qui ont été absorbés. Un plantage majeur qui est le suivant: if i == z[0]: donneDejaEnnergie = True
                           TypeError: 'Pays' object is not subscriptable 
     
     
Par la suite, l'erreur a été corrigée en changant ces lignes là : # Le voisin a de l'énergie à donner et le pays en difficulté a les ressources pour l'acheter
                        if surplus > 0 and COUT_ENER_EN_RESS*surplus >= p.ress:
                            i.ener_out.append([p, surplus/i.prod_ener])
                            p.ener_in.append([i, surplus/i.prod_ener])  
                            
                            
 Suite à cela, des derniers tests ont été établis, la satisfaction a été représentée visuellement à travers des graphiques, et le site a été finalisé.
