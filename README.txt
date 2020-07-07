Solving a maze
==============

ENGLISH

The idea here is to write a program to solve simple mazes. The mazes are given in 
a file and the program must read in the file, solve the maze and output the solution.
If no solution is possible the output should indicate this somehow. The program 
should be written to the following specification:
  
  - Arbitrary sized mazes should be handled
  - Valid moves are N, S, E, W (not diagonally)
  - All input will be clean, no validation is necessary
  - Any suitable language can be used although one of Java, C#, Python is preferred
  - The maze file format is described below with an example
  - The program should be tested on the sample mazes provided
  - Output should be written to the Standard Output/Console

================================================
==  ALL the sample mazes DO have a solution!  ==
================================================

The emphasis should be on code readability and simplicity. Runtime for all of the sample mazes should be <30 seconds.

Please email the solution in source code form, with short instructions on how to run.

Good luck!



Maze file format
================

The input is a maze description file in plain text.  
 1 - denotes walls
 0 - traversable passage way

INPUT:
<WIDTH> <HEIGHT><CR>
<START_X> <START_Y><CR>		(x,y) location of the start. (0,0) is upper left and (width-1,height-1) is lower right
<END_X> <END_Y><CR>		(x,y) location of the end
<HEIGHT> rows where each row has <WIDTH> {0,1} integers space delimited

OUTPUT:
 the maze with a path from start to end
 walls marked by '#', passages marked by ' ', path marked by 'X', start/end marked by 'S'/'E'

Example file:  
10 10
1 1
8 8
1 1 1 1 1 1 1 1 1 1
1 0 0 0 0 0 0 0 0 1
1 0 1 0 1 1 1 1 1 1
1 0 1 0 0 0 0 0 0 1
1 0 1 1 0 1 0 1 1 1
1 0 1 0 0 1 0 1 0 1
1 0 1 0 0 0 0 0 0 1
1 0 1 1 1 0 1 1 1 1
1 0 1 0 0 0 0 0 0 1
1 1 1 1 1 1 1 1 1 1

OUTPUT:
##########
#SXX     #
# #X######
# #XX    #
# ##X# ###
# # X# # #
# # XX   #
# ###X####
# #  XXXE#
##########


FRENCH

Le but ici est d'écrire un programme capable de résoudre des labyrinthes. Chaque labyrinthe se trouve dans un fichier,
le programme devra lire le fichier, résoudre le labyrinthe et afficher la solution.
Prévoir une sortie en cas de non solution.
Le programme doit respecter les spécifications suivantes:
  
  - Doit pouvoir résoudre des labyrinthes de n'importe quelles dimensions
  - Ne sont autorisés que les mouvements vers le Nord, Sud, Est et Ouest (pas de diagonale)
  - Chaque entrée est valide, pas de vérification nécessaire 
  - Peut-être réalisé dans le langage de votre choix même si Java, C#, Python sont recommandés
  - Chaque fichier d'entrée doit respecter le format décrit ci-dessous
  - Le programme doit être testé sur les échantillons fournis
  - La solution doit être affichée dans la console

================================================
==  TOUS les labyrinthes ont une solution  ==
================================================

Lisibilité et simplicité sont de mise. L'exécution de chaque labyrinthe doit durer <30 seconds.


Format d'entrée
================

L'entrée est un ficier texte.  
 1 - représente les murs
 0 - représente les chemins possibles

INPUT:
<WIDTH> <HEIGHT><CR>
<START_X> <START_Y><CR>		(x,y) coordonnées de départ. (0,0) est en haut à gauche and (width-1,height-1) est en bas à droite
<END_X> <END_Y><CR>		(x,y) coordonnées d'arrivée
<HEIGHT> lignes possédant <WIDTH> {0,1} colonnes dans un espace délimité

OUTPUT:
 le labyrinthe représentant le cheming entre le départ et l'arrivée
 les murs seront représentés par '#', les chemins qui ne mènent nulle part par ' ', le bon chemin par 'X', départ/arrivée par 'S'/'E'

Exemple:  
10 10
1 1
8 8
1 1 1 1 1 1 1 1 1 1
1 0 0 0 0 0 0 0 0 1
1 0 1 0 1 1 1 1 1 1
1 0 1 0 0 0 0 0 0 1
1 0 1 1 0 1 0 1 1 1
1 0 1 0 0 1 0 1 0 1
1 0 1 0 0 0 0 0 0 1
1 0 1 1 1 0 1 1 1 1
1 0 1 0 0 0 0 0 0 1
1 1 1 1 1 1 1 1 1 1

OUTPUT:
##########
#SXX     #
# #X######
# #XX    #
# ##X# ###
# # X# # #
# # XX   #
# ###X####
# #  XXXE#
##########