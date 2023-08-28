# EN_Instructions_setup_patch_clamp_cells
Instruction on how to use the setup for patching cell lines at the lab

---
title: "Patch clamp manual"
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
    \includegraphics[width=2in,height=2in]{https://github.com/LauraRobaye/Instructions_setup_patch_clamp_cells/issues/1#issue-1862803087}\LARGE\\}
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
# Matérial

https://github.com/LauraRobaye/Instructions_setup_patch_clamp_cells/issues/1#issue-1862803087
https://github.com/LauraRobaye/Instructions_setup_patch_clamp_cells/issues/2#issue-1864620487
https://github.com/LauraRobaye/Instructions_setup_patch_clamp_cells/issues/3#issue-1864627351
https://github.com/LauraRobaye/Instructions_setup_patch_clamp_cells/issues/9#issue-1864639067
https://github.com/LauraRobaye/Instructions_setup_patch_clamp_cells/issues/4#issue-1864629356
https://github.com/LauraRobaye/Instructions_setup_patch_clamp_cells/issues/5#issue-1864630577
https://github.com/LauraRobaye/Instructions_setup_patch_clamp_cells/issues/6#issue-1864631753

## Legend

1.  Burettes for external solution
2.  Screen for microscope settings
3.  Filters
4.  Support table for the dishes
5.  Mercury lamp
6.  Micromanipulator (arm)
7.  Headstage
8.  Pipette holder
9.  Oculary
10. Wheel for moving the dishes 
11. Macro-micrométric screw
12. Hearth
13. Micromanipulator housing
14. Shock absorbing table
15. Pump
16. Trash bottle
17. Grab bars for the dishes
18. Référence electrode
19. Objec lens
20. Switch for the microscope
21. Button for fluorescence
22. Button for transmission mode
23. Button for changing the light intensity (-)
24. Button for changing the light intensity (+)
25. Button for covering the light source
26. Button for changing the type of light source
27. Button for changing the type of light source
28. External solution arrival
29. Pump needle
30. Dish
31. Computer for the amplifyer
32. Computer screen for the camera
33. Computer screen for the amplifyer
34. Keyboard and mouse of the camera's computer
35. Keyboard and mouse of the amplifyer's computer
36. Command wheels for the micromanipulator
37. Tubbing for controling the micropipette's pressure
38. Computer for the camera
39. Amplifyer
40. Switch of the amplifyer
41. Switch of the interface
42. LED for signaling the overloads
43. Interface
44. Glass capillaries
45. "PULL" button
46. Switch for the pipette puller
47. Lid of the pipette puller
48. "ENTER" button
49. Safety latch
50. Screw for maintaining the glass capillaries
51. Spindle
52. Central piece containing the heating element
53. Spindle
54. Screw for maintaining the glass capillaries
55. Safety latch

\newpage

# 2. Getting started

## 2.1. Turning on the devices in that specific order

1.  The two computers 31) and 38)
2.  Turn on the amplifyer with the button 40)
3.  Turn on the interface with the button 41)
4.  Start *MultiClamp cmdr* (on screen 33))
5.  Start *pClamp* (on screen 33))
 **REMARK:**\
    If the computer does not find the devices when starting *MultiClamp cmdr*, shut down and start the interface and the amplifyer. If it is still not working, shut down the two device and the computer then start them again. If the graph at the bottom of the *pClamp* window is shown in pA instead of mV, press the *Reset* button on *MultiClamp cmdr*.
7.  Micromanipulator (housing 13))
8.  Microscope 20)
9.  Turn on the mercury lamp if the fluorecence is required 5). When it is swhitched on, we see it twinkeling in blue. Wait until it does not twinkle anymore for using it.
 **REMARK:**\
    Once the mercury lamp is turned on, you have to leave it turned on at least for two hours (you only shut it down when the experiment is already finished, not when you just take a small break or for lunch).
11.  Start *ZEN* (on screen 32)). Choose the *LIVE* mode for displaying the microscope field on the screen.

## 2.2. Preparing the setup

1.  Fill the styrofoam box with crushed ice (in the room where the fridge in which we store the external solution is located).
2.  De-freeze an internal solution eppendorf.
3.  Vortex the internal solution eppendorf and measure the solution's osmolarity (for making sure it will not damage the cells).
4.  Fill a 1 ml seringe with the internal solution without making bubbles.
5.  Put the eppendorf with the remaining solution in the crushed ice (you can write something on the lid of the eppendorf for not loosing it).
6.  Add a filter and then the needle to the seringe. Place it on the box by making the part with solution touching the ice to preserve is during the experiment.
7.  Fill the burette with external solution (it has to be at room temperature to avoid damaging the cells). If needed for the experiment, fill the other burettes with the corresponding solutions $\rightarrow$ Make sure that the burettes are closed at their base without filling them to avoid leaks.
8.  Purge the system with the solution. Start by placing the external solution arrival 28) in the trash beaker.
9.  Screw the lid on top of the trash bottle 16) and start the pump 29).
10. Place the pump needle 29) in the trash beaker.
11. Open the tap under each burette and then only let the solution from the last one on the right (you can adjust the rate flow at that time if needed).
12. Once the burette is almost empty, switch the tap of the burette just oon the left of the first one and so on until arriving to the one on the left. The aim is to have all the tubbings filled with external solution without any air bubbles.
13. Bring the dish containing the cells to patch in the cell culture lab.
14. Place the dish 30) in the bracket 17). Adjust the position is necessary and securize it with the modeling clay (be careful, the bracket move easily).
15. Place the external solution arrival in the dish (the tip should be placed under the surface of culture medium in the dish to avoid big drops arriving in the dish and making everithing move).
 **REMARK:**\
    As the external solution circulation works, the liquid flows out of the needle. To avoid splashing the setup and making saline bridges, always put a absorbant paper under the needle while moving it between the dish and the trash beaker.
17. Place the pump needle (exit) in the dish. Place it a tiny bit under the level of the external solution needle to avoid bubbles to fall and make everithing move (cf 5.).
 **REMARK:**\
    You have to make sure having as much distance as possible between the two needles in order to have a flux solution irrigating the whole dish. The recomanded debit is 1-2 ml.min^-1^. The adjustment is made at the start of the experiment with the roulette located on the last part of the tubbing. You can control if the debit is still correct by listening to the sound produced by the needle of the pump, you have to hear a constant sucking. It avoids interferences and too large liquid movements in the dish. It is also important to make sure a maximum of surface in the dish is available to move the pipette in it. Install the arrival, the exit and the reference electrode 18) on the outskirts of the dish.
**REMARK:**\
    It is important not to empty the burette(s) during the experiment, so you have to check the levels all along and fill them when necessary.
19. You should wait until the culture medium is fully replaced by the external solution before starting the reccordings (the liquid in the dish is not pink anymore but transparent).
20. At that tima do not forget to put the reference electrode 18) in the dish.

**REMARK:**\
  Over the course of the experiment it will be necessary to change the dishes (when cells will have a bad looking shape). At that time, you remove the reference electrode, the external solution entry needle (it goes in the trash beaker), you suck the external solution in the dish with the pump needle and put them in the trash beaker too $\rightarrow$ that way the flux does not have to be stop.

## 2.3. Making, filling and placing of the micropipettes

1.  Turn on the pipette puller with the button 46).
2.  Choose the program on the puller and press *ENTER* 48). For us the program is the 24.
3.  Take a capillary out of the plastic bag 44), make sure there is a tiny "thread" in it lumen.
4.  Open the puller's lid 47).
5.  Insert the capillary in one of the screw 50) or 54) and close it in order to keep the capillary in place without breaking it (do not force, there anti slippery material in it).
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
