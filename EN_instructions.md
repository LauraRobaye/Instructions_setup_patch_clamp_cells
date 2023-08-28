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
