# Instructions_setup_patch_clamp_cells
Instruction on how to use the setup for patching cell lines at the lab
---
title: "Manuel Patch clamp"
author: Laura Robaye
output:
  html_document:
    toc: true
    toc_depth: 4
  pdf_document:
    toc: true
    toc_depth: 4
header-includes:
  - \usepackage{titling}
  - \pretitle{\begin{center}
    \includegraphics[width=2in,height=2in]{Image_couverture.jpg}\LARGE\\}
  - \posttitle{\end{center}}
editor_options: 
  markdown: 
    wrap: sentence
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE, fig.align = 'center', 
                      message = FALSE, warning = FALSE)
```

```{r, include=FALSE}
setwd("~/Desktop/Doctorat/Patch_clamp_tutorial")
```

```{r, include=FALSE}
library(markdown)
library(tinytex)
```

## Légende

1.  Burettes pour solution externe
2.  Ecran des paramètres du microscope
3.  Filtres
4.  Table de support pour les dishes
5.  Lampe à mercure
6.  Micromanipulateur (bras)
7.  Headstage
8.  Pipette holder
9.  Oculaire
10. Roulette pour déplacer le dish
11. Vis macro-micrométrique
12. Terre
13. Boitier du micromanipulateur
14. Table sur amortisseurs
15. Pompe
16. Bouteille poubelle
17. Barres de maintien des dishes
18. Electrode de référence
19. Objectif
20. Interrupteur du microscope
21. Bouton pour la fluorescence
22. Bouton pour le mode transmission
23. Bouton pour le réglage de l'intensité de la lumière (-)
24. Bouton pour le réglage de l'intensité de la lumière (+)
25. Bouton pour occulter la source
26. Bouton de changement du type de source
27. Bouton de changement du type de source
28. Aiguille d'entrée de la solution externe
29. Aiguille de la pompe
30. Dish
31. Tour de l'ordinateur de l'ampli
32. Ecran de l'ordinateur de la caméra
33. Ecran de l'ordinateur de l'ampli
34. Clavier + souris de l'ordinateur de la caméra
35. Clavier + souris de l'ordinateur de l'ampli
36. Roulettes de commande du micromanipulateur
37. Tube pour la gestion de la pression dans la micropipette
38. Tour de l'ordinateur de la caméra
39. Ampli
40. Interrupteur de l'ampli
41. Interrupteur de l'interface
42. LED de signalement des overload
43. Interface
44. Capillaires en verre
45. Bouton "PULL"
46. Interrupteur de l'étireuse
47. Couvercle de l'étireuse
48. Bouton "ENTER"
49. Loquet de maintient
50. Vis pour maintenir le capillaire
51. Tige
52. Pièce centrale contenant la résistance
53. Tige
54. Vis pour maintenir le capillaire
55. Loquet de maintient

\newpage

# 2. Mise en route

## 2.1. Allumage des différents appareils dans l'ordre suivant

1.  Les deux ordinateurs 31) et 38)
2.  Allumer l'ampli avec le bouton 40)
3.  Allumer l'interface avec le bouton 41)
4.  Lancer *MultiClamp cmdr* (sur l'écran 33))
5.  Lancer *pClamp* (sur l'écran 33)) **REMARQUE:**\
    si l'ordinateur ne trouve pas les appareils quand on lance *MultiClamp cmdr*, éteindre l'interface et l'ampli puis les redémarrer. Si ça ne fonctionne toujours pas, les éteindre à nouveau et éteindre l'ordinateur en plus puis les rallumer tous. Si le graphe du bas de la fenêtre de *pClamp* est en pA au lieu de mV, appuyer sur le bouton *Reset* de *MultiClamp cmdr*.
6.  Micromanipulateur (boitier 13))
7.  Microscope 20)
8.  Lampe au mercure si on a besoin de la fluorescence 5). Quand elle est allumée on voit un clignotement bleu, attendre que la lumière ne clignote plus pour s'en servir **REMARQUE:**\
    une fois qu'on l'allume, il faut attendre au moins deux heures avant de l'éteindre (donc on ne l'éteint que quand on a vraiment fini, pas pour le temps de midi ou pour n'importe quelle pause).
9.  Lancer *ZEN* (sur l'écran 32)). Choisir le mode LIVE pour que l'écran affiche le champ du microscope

## 2.2. Préparartion du setup

1.  Remplir le bac de frigolite avec de la glace pilée (local où se trouve le frigo dans lequel on stocke la solution externe) et lui donner une forme de pente
2.  Sortir un eppendorf de solution interne congelée et le dégeler (entre ses mains).
3.  Vortexer l'eppendorf de solution interne puis mesurer son osmolarité (surtout utile si on a des soucis au patch pour éliminer le risque que ça soit ça qui abime les cellules)
4.  Remplir une seringue de 1 ml de solution interne en évitant les bulles
5.  Placer l'eppendorf contenant le reste de solution interne dans la glace (si le tube est nu, faire un petit repère au marqueur sur le capuchon pour ne pas le perdre dans la glace)
6.  Ajouter un filtre puis l'aiguille à la seringue et la placer aiguille vers le haut sur la glace
7.  Remplir la burette de solution externe 1) (si besoin remplir les autres burettes avec les solutions nécessaires à l'expérience) $\rightarrow$ Vérifier que la burette est fermée par la vanne à sa base avant de la remplir de solution externe
8.  Purger le système d'entrée des solutions. Placer l'aiguille d'arrivée de la solution externe 28) dans le berlin poubelle
9.  Visser le bouchon sur la bouteille poubelle 16 et allumer la pompe 15)
10. Placer l'aiguille de la pompe 29) dans le berlin poubelle
11. Ouvrir le robinet sous chaque burette puis ne laisser s'écouler que la solution de la burette située la plus à droite (on peut régler le débit d'écoulement à ce moment-là)
12. Une fois que la burette est presque vide, switcher le robinet d'ouverture de la burette juste à gauche et ainsi de suite jusqu'à arriver à la burette la plus proche du microscope. Le but est d'avoir les tuyaux remplis de solution externe sans bulles d'air.
13. Aller chercher le dish à patcher en culture cellulaire
14. Placer le dish de culture 30) sur le support 17). Régler l'espacement du support si nécessaire et sécuriser le placement avec un petite boule de plasticine (attention, les deux supports bougent très facilement)
15. Placer l'aiguille d'arrivée de la solution externe dans le dish (l'extrémité doit se situer juste en-dessous du niveau du milieu de culture pour éviter les grosses gouttes). **REMARQUE:**\
    comme la circulation de la solution externe fonctionne, il y a de la solution qui sort par l'aiguille. Pour ne pas éclabousser tout le setup, placer un papier absorbant sous l'aiguille jusqu'à atteindre le dish
16. Placer l'aiguille d'aspiration (sortie) dans le dish. Celle-ci doit idéalement se situer un peu au-dessus du niveau de l'aiguille d'entrée pour la solution externe. Ainsi la solution externe ne fera pas des grosses gouttes quand elle tombe (cf p5). **REMARQUES:**\
    Il faut veiller à éloigner le plus possible l'entrée et la sortie de sorte à avoir un flux de solution externe qui irrigue au maximum le dish. Le débit conseillé pour l'entrée de solution externe est de 1 à 2 ml/min. Le réglage se fait au début de la manip à l'aide de la roulette située le long du tuyau d'arrivée de la solution externe. Idéalement, il faut toujours entendre le bruit d'aspiration de la pompe, cela évite les interférences et les mouvements de liquides trop importants dans le dish. Il faut également veiller à laisser un maximum de surface disponible dans le dish pour la micropipette. Installer l'entrée, la sortie et l'électrode de référence le plus en périphérie du dish possible. **REMARQUE:**\
    il faut veiller à ne pas vider totalement la/les burette(s) au fil de la manip, penser à contrôler le niveau et à la/les remplir régulièrement.
17. Idéalement il faut attendre que le milieu de culture ait été remplacé par de la solution externe (le liquide rose aura été totalement remplacé par du transparent)
18. Placer l'électrode de référence 18) dans le bain

**REMARQUE:**\
Au fil de la session de patch, il faudra probablement changer de dish quand les cellules n'auront plus un aspect satisfaisant (elles n'apprécient pas trop d'être sorties de l'incubateur trop longtemps).
A ce moment-là, on retire l'électrode de référence, l'aiguille d'entrée (dans le berlin poubelle), on aspire le contenu du dish avec la pompe puis on place l'aiguille de la pompe dans le berlin poubelle $\rightarrow$ on ne doit donc pas couper le flux.

## 2.3. Fabrication, remplissage et mise en place des micropipettes

1.  Allumer l'étireuse avec le bouton 46)
2.  Entrer le numéro du programme d'étirement correspondant aux paramètres de l'expérience (ici c'est le programme 14) puis appuyer sur *ENTER* 48)
3.  Prendre un capillaire dans le sachet 44) et vérifier si la lumière du capillaire contient bien un petit « fil »
4.  Soulever le couvercle de l'étireuse 47)
5.  Insérer le capillaire dans un des supports de l'étireuse 50) ou 54) et le serrer de façon à maintenir le capillaire (pas besoin de serrer trop fort, c'est antidérapant)
6.  Libérer les deux supports 50) et 54) en appuyant sur les deux pièces 49) et 55) et approcher les deux supports de la pièce centrale 52) en approchant les deux tiges 51) et 53) du centre (les maintenir sinon elles repartent chacune de leur côté)
7.  Desserrer le support contenant le capillaire et faire glisser celui-ci de sorte qu'il soit centré (les deux extrémités doivent dépasser de la même façon de chaque côté)
8.  Serrer les deux supports sur le capillaire (ça doit le maintenir mais pas non plus l'écraser au point de l'éclater). A ce moment-là on peut lâcher les deux tiges.
9.  Fermer le couvercle 47)
10. Appuyer sur le bouton *PULL* 45)
11. Une fois que les deux micropipettes sont formées, les placer sur un support adéquat de sorte que rien n'entre en contact avec la pointe.
12. Une fois au setup, saisir une micropipette
13. Prendre la seringue de solution interne et en faire sortir un peu pour éviter les bulles et éliminer d'éventuels résidus qui se trouveraient dans l'aiguille
14. Insérer l'aiguille dans la micropipette le plus loin possible sans toucher la pointe (en pratique on l'insère jusqu'à l'endroit où elle commence à être étirée, on reste où le capillaire est bien cylindrique)
15. Commencer à injecter de la solution interne sans faire de bulle et retirer doucement l'aiguille en même temps que le liquide remplis la pipette tout en continuant d'appuyer sur le piston de la seringue
16. Remplir la pipette à environ 1/3 (maximum), il faut avoir assez de liquide pour que l'électrode touche le liquide quand la pipette est placée sur le headstage 7) (trop de solution interne mènerait à un débordement au moment de la fixation sur le headstage ce qui est mauvais pour l'appareil car cause des ponts salins et on ne veut pas ça pour le bruit ni pour le matériel)
17. Chasser les éventuelles bulles (des bulles dans la portion cylindrique de la pipette se chassent assez facilement contrairement à de mini-bulles dans la partie étirée de la pointe) en secouant fermement la pipette (attention à ne pas toucher la pointe) ou en donnant de petits coups à l'extrémité cylindrique de la pipette
18. Avant de placer la pipette sur le headstage (et donc de le toucher) placer les mains un court instant sur la plateforme métallique de la table du setup afin de décharger les mains d'éventuelles charges électriques
19. Insérer la pipette dans le headstage en veillant à introduire l'électrode dans la lumière de la pipette sans plier l'électrode). Tenir le headstage avec l'autre main afin d'éviter que le micromanipulateur prenne toute la force déployée à ce moment-là
20. Serrer la petite pièce en plexiglass pour fixer la pipette au support. Cela permet aussi de fermer hermétiquement le circuit
21. Tourner le headstage de façon à l'approcher du dish

**REMARQUE:**\
Sur l'ampli, il y a une petite LED en-dessous de l'inscription « Overload » 42).
Si celle-ci s'allume (en orange) il faut retirer et changer la pipette car cela signifie qu'il y a une surcharge dans l'électrode et c'est très mauvais pour l'appareil.
Il faut surveiller cette LED tout au long de l'expérience.
Si elle s'allume à répétition, c'est peut-être le signe de la présence de ponts salins $\rightarrow$ nettoyer le setup pour les enlever.

## 2.4. Sélectionner une cellule à patcher

1.  Choisir une zone qui sera facilement accessible pour la pipette. Si la cellule d'intérêt se trouve située trop près de la paroi gauche du dish ou tout près des entrée/sortie/électrode de référence, elle sera difficilement accessible avec la pipette donc l'idéal est de chercher vers le centre ou la paroi droite du dish.
2.  Une fois dans une zone facilement accessible, mettre au point et chercher une zone où les cellules ont un aspect optimal
3.  Sélectionner l'option pour la eGFP (si les cellules ont été transfectées avec le plasmide correspondant) avec les boutons 26) et 27).
4.  Activer l'émission de fluorescence avec le bouton 21)
5.  Si rien ne se passe (on ne voit pas des cellules avec le cytoplasme plus brillant que les autres), vérifier que l'intensité de la fluorescence est satisfaisante. Pour cela, utiliser les boutons 23) et 24) pour augmenter ou diminuer l'intensité.
6.  Sélectionner une cellule qui a le cytoplasme brillant, càd qui apparaît gris plus clair que les autres environnantes à l'écran. Si on est certains que la cellule est isolée des autres, la sélectionner pour le patch. Sinon repasser en visible pour s'assurer qu'elle est isolée ou du moins facile d'accès. Idéalement les HEK 293 ont une morphologie « irrégulière ». Elles peuvent être triangulaires ou avoir une forme « de limace » (elles ont des prolongements qui font penser à des antennes). Éviter les cellules qui ont un aspect trop sphérique avec des prolongements très petits et fins **REMARQUE:**\
    Il faut éviter de laisser la fluorescence trop longtemps sur les cellules, le fluorochrome se dégrade au fil de l'exposition donc si on veut garder des taux de fluorescence suffisant pour toute l'expérience, il faut y aller avec parcimonie.
7.  Repasser en visible. Appuyer sur le bouton 21) pour couper la fluorescence
8.  Revenir à l'option 6 avec le bouton 26) ou 27).
9.  Si l'intensité n'est pas satisfaisante, la régler avec les boutons 23) et 24)

# 3. Patcher une cellule

1.  Quand une cellule potentiellement intéressante a été repérée, la placer au centre de l'écran de *ZEN*.
2.  Sur *pClamp*, choisir « membrane test » I), cliquer sur *play* puis sur le mode « bath » L)
3.  Zoomer numériquement dessus avec la roulette de la souris 35) pour pouvoir mieux visualiser l'approche par l'électrode (à voir selon ses propres préférences)
4.  Placer la souris dessus, en son centre, pour avoir un repère visuel et ne plus la déplacer
5.  Approcher la pipette de la zone de champ du microscope (au-dessus de l'objectif 19)) à l'œil d'abord, tout en restant haut assez pour ne pas toucher le liquide dans le dish. Pour cela, rester en vitesse rapide avec le micromanipulateur.
6.  Une fois que l'on estime que la pipette est bien positionnée, la descendre assez pour que la pointe touche à peine le liquide
7.  Vérifier la résistance de la pipette. Pour cela, appuyer sur le bouton « AUTO » à côté de «pipette offset » C) sur *MultiClamp Comander*. Si la résistance se situe entre 2,5 et 5 M$\Omega$ c'est bien.
8.  Amener le focus du microscope le plus haut possible (tourner dans le sens qui indique « up » donc vers le fond de la cage de Faraday).
9.  Déplacer gentiment la pipette dans le plan horizontal pour essayer de la localiser avec les oculaires (ne pas la déplacer verticalement).
10. Une fois qu'on l'a repérée, essayer de l'amener au niveau du centre du champ pour pouvoir la localiser sur *ZEN*
11. Passer en vitesse lente sur le micromanipulateur et mettre au point la pointe de la pipette en jouant avec la position verticale de la pipette et la vis micrométrique. Amener la pointe de la pipette à l'endroit où on a positionné la flèche de la souris.
12. Descendre un peu le focus avec la vis macrométrique 11) en la tournant dans le sens indiqué «down » (vers soi).
13. Descendre ensuite la pipette afin de récupérer le focus sur sa pointe
14. Recommencer les étapes 12 et 13 jusqu'à ce que l'on voie qu'on approche des cellules mais avant de les avoir vraiment bien dans le focus.
15. Faire le focus sur la partie la plus haute des cellules et approcher la pipette très doucement en observant l'écran de *pClamp*. Quand on touche la cellule d'intérêt, on doit observer une augmentation de la résistance de la pipette mais surtout une diminution de la trace du courant sur la partie oscilloscope. A ce moment-là on arrête de descendre.
16. On saisit le tuyau 37) se terminant par un tip neuf (on change chaque jour) et on porte le tip à sa bouche
17. On donne une pression négative (on aspire) de façon douce et prolongée en surveillant la résistance. Le but est d'atteindre la valeur de 1 G$\Omega$. Si la résistance commence assez rapidement à augmenter, on peut arrêter d'aspirer quand on voit qu'elle atteint les 200-300 M$\Omega$ car normalement elle va aller au 1 G$\Omega$ d'elle-même. Pour aider pendant qu'on aspire on peut sélectionner « holding » B) sur *MultiClamp cmdr* et on le descend à -60 mV. Attention qu'il vaut mieux éviter mais si on le fait il faut penser à remettre le holding à 0 mV avant de lancer un protocole.
18. Pendant qu'on aspire ou que le G$\Omega$ seal se forme, on passe en mode « patch » M) sur *pClamp*.
19. Quand le G$\Omega$ seal est formé, compense les capacitances sur *MultiClamp cmd* en appuyant sur « Auto » à côté de « Cp Fast » E) puis de « Cp Slow » F). La trace de courant doit alors être plate (il n'y a plus les deux petits pics des capacitances) **REMARQUE:** si le G$\Omega$ seal est difficile à obtenir, que c'est trop lent à se produire ou qu'il faut aspirer trop fort ou trop longtemps, ça ne sert à rien de s'acharner, les meilleurs G$\Omega$ seal sont ceux qui arrivent le plus rapidement
20. Pour ouvrir la cellule en configuration whole cell, on aspire de façon brève et répetée mais un peu plus forte dans le tuyau 37) (la force peut être augmentée de succion en succion) jusqu'à ce que la trace contienne 2 pics assez grands (cf image avec *pClamp*). Pour juger que la cellule est bonne, on doit idéalement avoir une valeur de « Hold » entre 0 et -100 pA ainsi qu'une Ra \< 10 (\< 14 c'est acceptable).
21. Passer en mode « cell » N) sur *pClamp*
22. Sur *MultiClamp cmd*, cocher « Whole Cell » D) puis « Auto » puis décocher.
23. Si les paramètres semblent bons, appuyer sur l'icône *Stop* K) de la fenêtre de l'oscilloscope de pClamp. Aller sur « Open protocol » G), choisir le protocole qu'on veut utiliser, le lancer puis appuyer sur la boule rouge en haut H). Quand le protocole s'exécute, il y a un rectangle bleuté qui apparait autour de la boule rouge **REMARQUE:**\
    Si quand on lance le protocole le programme fait des siennes, on ferme *pClamp* (uniquement !!!) puis on le relance. Normalement quand il redémarre on a toujours la cellule en whole cell et ses paramètres reviennent. On peut alors relancer le protocole et ça doit fonctionner.
24. Pendant ce temps-là, prendre note des paramètres de la cellule (Cm, Rm, Ra, Tau et Hold) O) et du numéro de l'expérience (sur la fenêtre dans laquelle on voit le protocole).
25. Une fois le protocole terminé, on reset *MultiClamp cmdr* A), on ferme la fenêtre dans laquelle on voyait le protocole et on appuie sur l'icône *Play* J) de l'oscilloscope.
26. Changer de pipette. Pour la retirer, repasser le micromanipulateur en vitesse élevée et la sortir verticalement. Faire pivoter le headstage vers la gauche et changer de pipette.

**REMARQUE:**\
dès qu'on a touché une cellule avec la pipette ou qu'on a touché le fond du dish avec la pointe (on voit des débris de verre), il faut la changer.
De même s'il y a une petite bulle ou une crasse dans la pipette, on change.

# 4. Nettoyage du setup

1.  Éteindre tous les appareils en terminant par l'ordinateur qui contient les softwares *Multiclamp cmdr* et *pClamp* SAUF la pompe 15)
2.  Retirer son tuyau et le ranger
3.  Retirer le tip du tuyau 37) et le jeter
4.  Fermer la/les burette(s) 1) avec la/les vanne(s) à la/leurs base(s)
5.  Aspirer le reste de solution externe se trouvant dans le dish puis jeter le dish de culture dans la poubelle B2 (jaune)
6.  Remplir un berlin de rinçage d'eau déminéralisée et y tremper l'électrode de référence quelques fois puis l'essuyer avec un papier. La replacer sur la plateforme du microscope sur un papier absorbant.
7.  Placer les aiguilles d'entrée et de sortie dans le berlin poubelle et ouvrir la roulette de réglage au maximum pour avoir le plus grand flux possible
8.  Fermer les robinets sous la/les burette(s) et les retirer
9.  Vider le contenu de la/les burette(s) dans l'évier (s'il y a des drogues, les vider dans la tourie à liquides spéciaux) et les rincer à l'eau MilliQ (robinet avec le collant rouge)
10. A l'aide de la seringue remplie d'eau MilliQ (en mettre dans le berlin à eau pour que ça soit plus simple), rincer le système de robinets sous les burettes. Commencer par celle qui est plus proche du microscope pour terminer par celle qui est la plus à droite. Vider 4-5 seringues dans chaque entrée
11. Placer l'aiguille d'entrée de la solution externe sur le papier absorbant à côté du microscope.
12. Aspirer le reste du contenu du berlin poubelle avec la pompe puis placer l'aiguille sur le papier absorbant
13. Éteindre la pompe
14. Vider le contenu de la bouteille poubelle dans la tourie liquides spéciaux puis rincer la bouteille 3 fois avec de l'eau courante (verser le 1e rinçage dans la tourie à liquides spéciaux, surtout si on a utilisé des drogues).
15. Replacer la bouteille à côté du setup sans la reboucher pour qu'elle sèche
16. Essuyer le bouchon de la bouteille et donc les seringues fichées dedans avec un papier absorbant pour éviter le développement de moisissure.
17. Jeter les pipettes usagées du grand berlin poubelle dans la poubelle B2 (jaune).
18. Vider la glace dans l'évier et jeter l'eppendorf de solution externe à la poubelle
19. Vider puis nettoyer la bouteille de solution externe, la seringue et l'aiguille pour remplir les pipettes. Les ranger à leur place. Jeter le filtre.




