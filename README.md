 # Bureau d'Etude
 ## Modélisation de Systemes Robotiques
 Oualid El Abdaoui, Alexandre Langlade, Aniss Louahadj, Alexandre Malgouyres, Clement Truillet   
 *2A SRI UPSSITECH - 2020*   
 ---
 
 ## Introduction
 Ce programme a été réalisé dans le cadre d'un bureau d'étude encadré par M.Taix.   
 Son seul est unique but et de representer les variations des parametres d'un bras manipulateur RPR en position, vitesse et acceleration en fonction du temps lors d'un deplacement du repere Outil d'un point A vers un point C en passant par un point B. 
 
 ## Dépendances
 Le bon fonctionnement de ce programme necessite *Python 3* ainsi que les librairies *MatPlotLib* et *Numpy*.
 
 ## Utilisation
Les positions des points *A*, *B* et *C* sont à entrer dans le fichier *position* sous le format suivant :
```python
A:
 pos:
  x:0.5
  y:0
  z:2
B:
 pos:
  x:0
  y:0
  z:1.5
 vit:
  x:1
  y:0
  z:0
  rx:0
  ry:0
  rz:0
C:
 pos:
  x:-2
  y:-2
  z:2
```

Il est possible d'ajouter un ou plusieurs points de passage en ajouter des points dans le format suivant entre les points B et C :
```python
B2:
 pos:
  x:0
  y:0
  z:1.5
 vit:
  x:1
  y:0
  z:0
  rx:0
  ry:0
  rz:0
```
 /!\ Veuillez respecter l'indentation du document. 
 
 
 Pour lancer le programme, il suffit de lancer le fichier *main.py*
 Si les parametres sont compatibles avec le bras manipulateur, une fenetre MatPlot s'ouvrira.
 Sinon, un message d'erreur s'affichera.  
 
 ### Repere Outil
 Une modification du repere outil est possible en changeant le contenu du fichier *t34* representant la matrice T34 du modele du BM.
 
 ### Parametres du bras manipulateur
Une modification des parametres du BM (butées, vitesses et accélarations maximales) est possible en changeant le contenu du fichier *robot_param*.
 
 
 ---
 Tout les tests ont étés effectués dans un environnement *Python 3.8* dans les IDE *Spyder* et *PyCharm*