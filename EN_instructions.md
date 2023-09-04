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
19. Object lens
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
5.  Insert the capillary in one of the screw 50) or 54) and close it in order to keep the capillary in place without breaking it (do not force, there is non-slippery material in it).
6.  Press the two pieces 49) and 55) to free the supports 50) and 54) and approach the two supports to the central piece 52) by approaching the two spindles 51) and 53) to the center (hold them to avoid they go back to their initial position).
7.  Loosen the support holding the capillary and make it slide in order it is positioned in the middle of the device (the two ends of the capillary should be at the same distance from the center of the device).
8.  Tighten the two supports on the capillary (it has to be maintain on its place but no need to crush it). At that moment you can remove your fingers from the two spindles.
9.  Close the lid 47).
10. Press the *PULL* button 45).
11. Once the two micropipettes are formed, remove them from the puller and place them on an appropriate support. Make sure nothing touch the tip of them, they would be useless.
12. When back at the setup, take a micropipette.
13. take the internal solution seringe and let a few droplets come out of it (it prevents from having some durt and residues entering the micropipette).
14. Insert the needle in the micropipette. You have to reach the part where it starts to shrink but without touching the tip. Stay where the capillary is still cylindrical.
15. Start to inject the internal solution without making any bubbles and slowly remove the needle as the pipettes is filling.
16. The micropipette should only be filled to 1/3 (maximum!). There must be enought liquid to touch the silver electrode when the pipette is fixed to the pipette holder 7). If there is too much internal solution, it will leak everywhere in the pipette holder and produce sline bridges, which is bad for the devices and the recordings.
17. Remove the bubbles if there are some by shaking vigourously the pipette while holding it by the open end or giving it tiny shocks on the open end (be careful not to touch the tip of the pipette).
18. Before putting the pipette on the pipette holder, make sure you briefly touch the anti-vibration table to make sure you do not carry electrostatic charges to the headstage.
19. Insert the micropipette in the pipette holder while making sure you do not blend the silver electrode. Put one of your hand on the pipette holder while placing the pipette to avoid damaging the micromanipulator.
20. Screw the small plexiglass part to maintain the pipette in the pipette holder. This way the circuit is closed and air can not leak.

**REMARK:**\
There is an orange LED on the amplifyer under the *OVERLOAD* writting 42).
If the LED lights up, you have to remove the pipette and change it because it means there is an overload on the electrode and it it really damagefull for the device.
Make sure you keep an eye on that LED during the course of the experiment. If it keeps lighting up, it may be a sign there are saline bridges $\rightarrow$ clean the setup to get rid of them.

## 2.4. Selecting a cell to patch

1.  Choose an area which the pipette can reach easily. If the cell is too close to the left ridge or too close to the external solution entry/the pump/the reference electrode, it would be too tricky or even impossible to patch. You should idealy search for a cell on the right part of the dish.
2.  Once in an accessible area, find some cells with a good looking aspect.
3.  Select the eGFP mode on the microscope (if the cells are tranfected with the corresponding plasmid) with buttons 26) and 27).
4.  Turn on the fluorescence with the 21) button.
5.  If nothing happens (you do not see cells with brighter cytoplasm tahn the others), check if the fluorescence is at a prpoper value. For that purpose, use the 23) and 24) buttons to increase or decrease the intensity.
6.  Select a cell with the bright cytoplasm, it should appear in a brighter grey shade than the surrounding cells on the coputers's screen. If the cell is isoleated enought from the surrounding cells, select it for patching. If it is not the case, swith to visible light to make sure it is isolated and easy to patch. Idealy, HEK 293 cells have an irregular morphology: they can have a triangular or "slug" shape (they are elongated with two antennea). Try to avoid cells which are to spherical or with really tiny and thin extentions.
 **REMARK:**\
    Avoid letting the fluorescence on the cells for too long, it will degrade the fluorochrome. So if you want to keep the fluorescnce at correct rates for the experiments, do not turn it on for too long.
8.  Switch back to visible mode. Press the 21) button to shut down the fluorescence.
9.  Switch back to mode 6 with button 26) or 27).
10.  If the intensity is not satisfying, tune it with the 23) and 24) buttons.

# 3. Patch a cell

1.  When a cell seem promising, place it at the center of the vield visible on the *ZEN* screen.
2.  On *pClamp*, choose the *Membrane test* I) option, clic on *Play* and then on the *Bath* mode L).
3.  Numerically zoom on it with the mouse 35) in order to have better view when you will approach the cell with the pipette.
4.  Place the pointer of the mouse on the center of the cell in order to have a landmark and do not move the mouse after.
5.  Place the pipette as close as possible to the centrer of the microscope field (on top of the object lens 19)) while still staying hight enough to aivoid touching the surface of liquid. For this approach, use the micromanipulator in hight speed mode.
6.  Once you think the pipette is correctly placed, bring it down to make its tip touch the external solution.
7.  Check the value of resistance for the pipette. To do so, click on the *Auto* button on the side of *Pipette offset* C) on *MultiClamp Cmdr*. If the value of resistance is between 2.5 and 5 M$\Omega$, it is optimal.
8.  Bring the focus as hight as possible (turn the wheel in the "up" direction, towards the bottom of the Faraday cage).
9.  Gently move the pipette in the horizontal plan to localize it in the occularies (do not move it vertically).
10. Once you have spot it, bring it to the centrum of the field to localize it in the *ZEN* window.
11. Change the micromanipulator to fast speed and focus on the tip of the pipette by moving it vertically to find the focus and got the help of the macrometric screw. When the tip of the pipette is in the focus field, place it where you put the pointer of the mouse previously.
12. Turn the macrometric screw 11) a bit to move the focus a bit below the position of the tip of the pipette (turn the macrometric screw as indicated by the arrow saying *"Down"* in your direction).
13. After that, lower the position of the pipette a tiny bit in order to place its tip it in the "new" focus plan.
14. Start again the steps 12. and 13. until you start seeing the shape of the cells in the bottom of the dish (you can see them as dark, almost black shadows in the bottom of the dish). At that moment be really carefull and do not move the pipette for the moment.
15. Make the focus on the top layer of the cells and lower the pipette really slowly and carefully while looking at the *ClampFit* window. You will know when you touch the cell of interest when you observe an increase of the value of resistance of the piepette but, even more evident, when current trace on the the screen decreases. At that precise moment, you stop lowering the pipette.
16. Grab the tubbing 37) which ends with a pipette tip (you change it between every person using the set up) and bring the tip-ending part to your mouth.
17. Apply a really gentle and continuous negative pressure (sucking) while keeping an eye on the resistance value. The aim is to make the resistance reach the 1 G$\Omega$ value. If the resistance rises fast, you can stop applying the negative pressure when the resistance reaches 00-300 M$\Omega$. At that moment it will probably reach the 1 G$\Omega$ by itself. At that moment you can apply a holding value of -60 mV B) in *MultiClamp cmdr*. On donne une pression négative (on aspire) de façon douce et prolongée en surveillant la résistance. Le but est d'atteindre la valeur de 1 G$\Omega$. If the cell is slow to reach the 1 G$\Omega$ seal, you can help it by keeping applying the negative pressure really slowly.
18. While applying the negative pressure, change the mode on *pClamp* from *"BATH"* to *"PATCH"* M).
19. After the 1 G$\Omega$ is reached, compensate the capacitances on *MultiClamp cmdr* by pressing the *Auto* button on the side of *Cp Fast* E) and *CpSlow* F). The current trace should be totally flat at that moment (we removed the two capacitances peaks from the signal).
 **REMARK:** It the G$\Omega$ seal is difficult to reach, or too slow, if it requires to apply the negative pressure for too long, it is probably the sign that the cell is not a good candidate for the experiment so move on, change the pipette and try with another pipette. The best 1 G$\Omega$ seals are supposed to be reached really fast.
21. To reach the whole cell configuration, apply a fast and kind of strong negative pressure on the tubbing. You will probably have to do it a few times in order to open the cell. You will know it is open when the trace on *pClamp* shows two big peaks (see on th images below).
22. Change the mode to *"CELL"* N) on *pClamp*. At that moment you can judge the quality of the cell by looking at the *Hold* value on *pClamp*. This value should be comprised between 0 and -100 pA and the Ra value should ideally be situated between 10 to 14 M$\Omega$.
23. Sur *MultiClamp cmd*, cocher « Whole Cell » D) puis « Auto » puis décocher.
24. Si les paramètres semblent bons, appuyer sur l'icône *Stop* K) de la fenêtre de l'oscilloscope de pClamp. Aller sur « Open protocol » G), choisir le protocole qu'on veut utiliser, le lancer puis appuyer sur la boule rouge en haut H). Quand le protocole s'exécute, il y a un rectangle bleuté qui apparait autour de la boule rouge **REMARQUE:**\
    Si quand on lance le protocole le programme fait des siennes, on ferme *pClamp* (uniquement !!!) puis on le relance. Normalement quand il redémarre on a toujours la cellule en whole cell et ses paramètres reviennent. On peut alors relancer le protocole et ça doit fonctionner.
25. Pendant ce temps-là, prendre note des paramètres de la cellule (Cm, Rm, Ra, Tau et Hold) O) et du numéro de l'expérience (sur la fenêtre dans laquelle on voit le protocole).
26. Une fois le protocole terminé, on reset *MultiClamp cmdr* A), on ferme la fenêtre dans laquelle on voyait le protocole et on appuie sur l'icône *Play* J) de l'oscilloscope.
27. Changer de pipette. Pour la retirer, repasser le micromanipulateur en vitesse élevée et la sortir verticalement. Faire pivoter le headstage vers la gauche et changer de pipette.
**REMARQUE:**\
dès qu'on a touché une cellule avec la pipette ou qu'on a touché le fond du dish avec la pointe (on voit des débris de verre), il faut la changer.
De même s'il y a une petite bulle ou une crasse dans la pipette, on change.

https://github.com/LauraRobaye/Instructions_setup_patch_clamp_cells/issues/7#issue-1864632930
https://github.com/LauraRobaye/Instructions_setup_patch_clamp_cells/issues/8#issue-1864638043

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
