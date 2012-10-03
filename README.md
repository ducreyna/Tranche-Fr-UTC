A)  Objectif

L’objectif ici est de découvrir et d’utiliser les technologies qui ont attrait à la réalité virtuelle à travers la création d’un jeu accessible au plus grand nombre. L’intérêt est d’interagir avec plusieurs interfaces de réalité virtuelle telles que la wiimote, le gant à fibre optique et la stéréoscopie 3D avec tracking afin de rendre le projet le plus immersif possible. Toute cette application sera créée à l'aide du logiciel Virtools.

Ce projet est tiré de l’application pour Smartphone Fruit Ninja (http://www.fruitninja.com/), qui consiste à couper des fruits au vol en réalisant le maximum de combos durant un temps imparti. Il faut également noter que le joueur sera soumis à des pièges lors du lancement des fruits, ces pièges consisteront à des bombes. Si le joueur a la malchance d’en couper un le jeu prendra fin immédiatement.

Notre jeu mettra en scène deux joueurs en écran splitté. Chaque joueur sera face à l’écran où un projecteur affichera les éléments de jeu ainsi que l’avatar de son adversaire : le katana d’un côté pour le “trancheur” et la main de l’autre pour le “lanceur”. Ces images seront restituées en utilisant la stéréoscopie. Les utilisateurs auront alors à porter des lunettes passives pour appréhender la distance entre eux et les éléments de jeu. De plus, chaque joueur aura un but spécifique dans la partie. En effet, il y en aura un qui lancera des fruits (ou des bombes) et l’autre qui devra les couper au vol avant qu’ils ne le dépassent. Le joueur qui lancera le fruit devra d’abord le choisir en le saisissant avant de le lancer.


B)  Scénario

  1.	Niveau 1

Ce niveau a pour but de former le joueur au lancé de fruit et au maniement du katana. C’est pourquoi nous avons pensé proposer au joueur différentes sessions d’entraînement avant de se lancer dans le duel:

      1.1.	Session Maniement au sabre (avec la wiimote): 
  Elle consiste à couper tous les fruits qui se présentent à l’écran avant la fin du temps imparti. Le joueur se trouve face à un mur qui va servir de Grid pour lancer les fruits (ou bombe). Les fruits sont chargés dynamiquement à partir des ressources et suivent une trajectoire elliptique respectant les lois physiques. Ils peuvent par exemple rebondir sur le sol et être freinés dans leur course. Le katana, quant à lui, sera tracké, la position et l’orientation de celui-ci sont établies grâce la constellation fixée sur la wiimote. 
  Le katana est manipulé comme-ci si le joueur lui-même tenait le manche afin d’avoir la sensation d’immersion. Quand le joueur tranche un fruit, celui-ci explose et ralentit sa course afin de rendre la simulation la plus réelle possible. Nous avons également ajouté des sons qui simulent le bruit du sabre lors de ses mouvements dans l’air, le bruit d’une grenade qui explose etc… Un score est également mis en place dans la scène, à chaque fruit correspond un certain nombre de points qui seront ajoutés (ou retirés si c’est une grenade) lorsque celui-ci est tranché par le katana.

      1.2.	Session Lancement (avec le gant): Elle consistera à lancer le fruit vers une cible qui apparaitra à l’écran. L’environnement sera sensiblement le même que celui de l’entrainement katana, c’est à dire le ciel, un sol et un mur qui fera office de support pour la cible. L’appréhension du fruit dans le monde virtuel est assurée par une main virtuelle contrôlée par l’utilisateur grâce au gant à fibre optique tracké. Le joueur doit saisir le fruit à l’aide de cette main et ensuite le lancer à travers la cible (symbolisée par un anneau). Cette scène disposera également d’un compte à rebours et d’un champ score.
  Elle consistera à lancer le fruit vers une cible qui apparaitra à l’écran. L’environnement sera sensiblement le même que celui de l’entrainement katana, c’est à dire le ciel, un sol et un mur qui fera office de support pour la cible. L’appréhension du fruit dans le monde virtuel est assurée par une main virtuelle contrôlée par l’utilisateur grâce au gant à fibre optique tracké. Le joueur doit saisir le fruit à l’aide de cette main et ensuite le lancer à travers la cible (symbolisée par un anneau). Cette scène disposera également d’un compte à rebours et d’un champ score.

  2.	Niveau 2

Dans ce niveau, c’est le jeu comme nous l’avons présenté plus haut dans le cahier des charges. C’est une unification des scènes d’entrainement dans une même scène, ainsi le joueur ne sera pas perdu et saura quoi faire pour gagner. L’écran est splitté en deux, un joueur lance un fruit (ou une bombe) tandis que l’autre voit le fruit approché et doit le couper au passage. De plus, les deux joueurs bénéficie tous les deux de la stéréoscopie trackée, l’un passive et l’autre active. Nous utilisons deux ordinateurs reliés chacun à un vidéoprojecteur. Chaque couple ordinateur/vidéoprojecteur est utilisé pour un joueur. Nous synchronisons les deux ordinateurs et les données transmises entre eux via le réseau.


  3.	Niveau 3

Un mode “Extrême” est rajouté, où chaque joueur peut lancer et trancher des fruits (ceux lancés par l’adversaire). Nous gardons les mêmes interfaces (wiimote + gant) en intégrant un moyen pour chacune de passer du mode “trancheur” au mode “lanceur” rapidement (et vice versa).
