

# Dynamiques de dépendance inter-pays
**ARE DYNAMIC**
[**View on GitHub**](https://github.com/NathanSauret/ARE_Dynamic_Nathan_Najla_Claude)

![Image du monde](https://ec.europa.eu/cefdigital/wiki/download/attachments/106235155/world-1264062_1920.jpg?version=1&amp;modificationDate=1561369833246&amp;api=v2)

### Introduction
Nous avons mené une recherche portant sur l'analyse de la stabilité potentielle résultant de la dépendance énergétique entre pays, et de sa généralisation entre groupes donnés. Les relations que les puissances entretiennent au niveau des ressources peuvent jouer un rôle déterminant dans l'évolution économique d'un pays. Elles sont indispensables à sa santé économique, expriment son influence et son degré de présence sur le marché international. Nous avons ainsi cherché à déterminer et modéliser les principaux facteurs contribuant à la stabilité générale d'un ensemble de pays ou menant à un déséquilibre global.

#### Description synthétique du projet

##### Problématique :
La dépendance énergétique entre pays amène-t-elle à une stabilité générale ?

##### Hypothèse principale :
L'hypothèse de notre projet informatique est que l'évolution des échanges dans une micro-économie inter-pays basée sur des règles simples tendra généralement vers une stabilité. En d'autres termes, la majorité des cas aboutiront à une situation où les échanges se stabilisent. Nous prévoyons que les variations seront limitées et que les conditions seront favorables à la pérennité de l'économie. Cette hypothèse se base sur l'idée que les règles simples seront suffisantes pour équilibrer les échanges entre les différents pays impliqués dans le système. Nous allons tester cette hypothèse en développant un modèle informatique et en observant son évolution sur une période donnée.

##### Objectifs :
- Observer les potentielles stabilités et les conditions initiales qui y amènent
- Identifier les facteurs qui influencent les flux commerciaux entre les pays, tels que la distance géographique, les différences de tailles ou les barrières financières.
- Étudier la résilience des pays isolés et non isolés.

##### Règles de modélisation :
- La production d'énergie
- La consommation d'énergie
- Les ressources
- Le prix de l'échange
- La limite de tour non-stable avant fusion
- Le pourcentage d'énergie donnée lors des échanges
- Dimension de la grille

##### **Explication des règles de modélisation :**
Au commencement de la simulation, chaque pays dispose aléatoirement d'un niveau de production, de consommation ainsi que de ressources limitées dans les paramètres définis préalablement. À chaque itération suivante, le niveau de ressources de chaque pays augmente en raison de sa production. En cas de sur-production (production supérieure à la consommation), un pays peut procéder à un échange avec un autre pays voisin disposant de la production excédentaire, en échange de ressources disponibles. Toutefois, si un pays demeure en situation de sous-production pendant un nombre de tours déterminé en amont de la simulation, il sera absorbé par un pays voisin, sous réserve que ce dernier dispose d'une production suffisante.

### Présentation structurée des résultats



![Courbe](https://media.discordapp.net/attachments/1071034292467159130/1096073386511323332/2023-04-13_16_01_50-NVIDIA_GeForce_Overlay_DT.jpg?width=1082&height=606)
**La partie terminal de commande**

![Image](https://media.discordapp.net/attachments/1071034292467159130/1096073551167098920/2023-04-13_16_02_07-NVIDIA_GeForce_Overlay_DT.jpg?width=735&height=606)
**En début de simulation**

![Image](https://media.discordapp.net/attachments/1071034292467159130/1096073600148197448/2023-04-13_16_03_08-NVIDIA_GeForce_Overlay_DT.jpg?width=730&height=606)
**En milieu de simulation**

![Image](https://media.discordapp.net/attachments/1071034292467159130/1096073665478672384/2023-04-13_16_03_16-NVIDIA_GeForce_Overlay_DT.jpg?width=730&height=606)
**La stabilité en milieu de simulation**

![Image](https://media.discordapp.net/attachments/1071034292467159130/1096074077380296724/2023-04-13_16_06_41-NVIDIA_GeForce_Overlay_DT.jpg?width=732&height=606)
**En fin de simulation**

![Image](https://media.discordapp.net/attachments/1071034292467159130/1096074153146208327/2023-04-13_16_06_49-NVIDIA_GeForce_Overlay_DT.jpg?width=731&height=606)
**La stabilité en fin de simulation**



On peut également observer la simulation sur différentes échelles : 

![Image](https://media.discordapp.net/attachments/1071034292467159130/1096074387792330822/2023-04-13_16_07_44-NVIDIA_GeForce_Overlay_DT.jpg?width=732&height=606)
**En 5x5**

![Image](https://media.discordapp.net/attachments/1071034292467159130/1096074423137747015/2023-04-13_16_08_02-NVIDIA_GeForce_Overlay_DT.jpg?width=733&height=606)
**En 20x20**

![Image](https://media.discordapp.net/attachments/1071034292467159130/1096075949226864671/2023-04-13_16_09_41-NVIDIA_GeForce_Overlay_DT.jpg?width=733&height=606)
**Et même en 100x100**



Nous avons par la suite modélisé la satisfaction des pays suite aux résultats à l'aide de graphes : 

![Image](https://media.discordapp.net/attachments/1071034292467159130/1096382371009409165/cons_ener.png?width=1203&height=606)


![Image](https://media.discordapp.net/attachments/1071034292467159130/1096382371252674590/cout_ener.png?width=1203&height=606)


![Image](https://media.discordapp.net/attachments/1071034292467159130/1096382371571433562/pourcent_max.png?width=1203&height=606)

![Image](https://media.discordapp.net/attachments/1071034292467159130/1096382371844075560/prod_ener.png?width=1203&height=606)


![Image](https://media.discordapp.net/attachments/1071034292467159130/1096382372368351262/taille_grille.png?width=1203&height=606)


![Image](https://media.discordapp.net/attachments/1071034292467159130/1096382372649382048/tour_nonstable.png?width=1203&height=606)


## Analyse des résultats : 
En procédant à l'analyse globale des résultats, il apparaît que les disparités économiques inter-pays tendent à s'estomper davantage, sans pour autant parvenir à atteindre le niveau maximal de satisfaction dans chacun des pays. La satisfaction observée varie selon les paramètres pris en compte, ce qui donne des résultats plus ou moins distincts. Par ailleurs, il est à noter que les différents pays atteignent un seuil de stabilité différent approximativement au même moment. De plus, les graphiques présentant la satisfaction en fonction de la taille de la grille illustrent une certaine proximité entre eux.
### Lien vers page de blog :
[C'est ici !](blog.md)

### Membres du groupe
- Nathan Sauret
- Claude Chibout
- Amira Rachdi
- Najla El Kentaoui

### Bibliographie :
1. [« Indépendance énergétique ». Wikipédia](https://fr.wikipedia.org/w/index.php?title=Ind%C3%A9pendance_%C3%A9nerg%C3%A9tique&oldid=200590596)
2. [Simple economic model (MATLAB) - LiteratePrograms. ](https://literateprograms.org/simple_economic_model__matlab_.html)
3. [Simard-Casanova, Olivier. « Les Nouveaux Usages de La Simulation Informatique En Science économique ». The Conversation, 15 janvier 2017](https://theconversationhttps://www.academia.edu/10676359/Agent_based_model_of_a_simple_economy.com/les-nouveaux-usages-de-la-simulation-informatique-en-science-economique-61536)
4. [Macal, Charles M., et Michael J. North. « Agent-based modeling and simulation ». Proceedings of the 2009 Winter Simulation Conference (WSC), 2009](https://www.researchgate.net/publication/216813135_Agent-based_modeling_and_simulation)
5. [ ACE: A Completely Agent-Based Modeling Approach (Tesfatsion)](http://www2.econ.iastate.edu/tesfatsi/ace.htm)
6. [valentinaalto. « Understanding Agent Based Model with Python ». Data Science Chalk Talk, 7 juin 2020](https://datasciencechalktalk.wordpress.com/2020/06/07/understanding-agent-based-model-with-python/)
