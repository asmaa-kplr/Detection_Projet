# Roboflow

Roboflow est un outil qui facilite la tâche de la vision par ordinateur dans le domaine de l'apprentissage en profondeur. Il permet aux développeurs de créer leurs applications de vision par ordinateur, quel que soit leur niveau de compétence ou d'expérience. Il prend en charge les modèles de détection et de classification d'objets. Cet outil peut faire ce qui suit :

* Annotation de jeux de données
* Prétraitement des jeux de données
* Fusion de projets/jeux de données
* Vérification de la santé du jeu de données
* Exportation des jeux de données
* Entraînement du modèle

![image](https://user-images.githubusercontent.com/123757632/234112416-bace7afb-e916-43ef-a315-572ae010a73e.png)

## 1 . Créer un nouveau projet
Dans le workspace Roboflow, il faut cliquer sur le bouton "Create New Project", sélectionner "Object Detection (Bounding Box)" comme type de projet, spécifier "personne" pour la question "what are you detecting ?", et enfin donner le nom de "Detection de Personnes" au projet.

![image](https://user-images.githubusercontent.com/123757632/234117152-06bacdda-b10c-45b4-8cdf-a27c945ca0ea.png)

il reste qu'a cliquer sur le bouton "Create Private Project" pour finaliser le projet .

## 2 . Importation de donnée a partir d'une video

![image](https://user-images.githubusercontent.com/123757632/234117576-fdd2d79d-6bad-48e7-bcfe-b12e9e2f9045.png)

 Dans l'input "Import Youtube Video" , il faut saisir le lien suivant et cliquer sur l'icône "Flèche" située à droite : https://www.youtube.com/watch?v=YzcawvDGe4Y&t=3s&ab_channel=GKorb 

![image](https://user-images.githubusercontent.com/123757632/234118171-613f5aba-2da3-4831-8cb0-d46619ca9039.png)

 
## 3 . Découpage de la vidéo en images 

Maintenant, après avoir téléchargé la vidéo, il faut choisir le nombre d'images que Roboflow va découper à partir de la vidéo précédente. Dans le cadre de cet atelier, on choisira "10 images". Toutefois, pour obtenir un ensemble de données plus robuste, il est recommandé de choisir un nombre plus élevé. Il faut cliquer sur le bouton "Choose Frame Rate".

![image](https://user-images.githubusercontent.com/123757632/234118442-47f0e116-da28-4e5b-925e-7050133020eb.png)

Il faut enregistrer l'ensemble de données en cliquant sur le bouton "Save and Continue" situé tout à droite, puis sur le bouton "Assign Images". 
Ensuite, il faut cliquer sur la première image pour commencer l'annotation.

## 4 . Annotation des images

Roboflow prend en charge différents types d'annotations, notamment :

* Boîte englobante (Bounding box) : qui encadre l'objet avec un rectangle
