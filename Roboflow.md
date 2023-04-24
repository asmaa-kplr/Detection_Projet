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

![image](https://user-images.githubusercontent.com/123757632/234118928-68a17e05-d447-4e6a-b08b-662220fa1174.png)

* "Smart polygon" permet de dessiner rapidement des polygones (ou des formes avec plusieurs côtés) autour d'objets complexes, tels que des voitures ou des bateaux, en suivant automatiquement les contours de ces objets.

![image](https://user-images.githubusercontent.com/123757632/234130279-d2cfada1-0715-48b3-8c3a-fb2eaa004251.png)

* "Label Assists" est un outil d'assistance à l'étiquetage qui suggère des étiquettes possibles en temps réel en fonction du contexte de l'image, ce qui peut aider les utilisateurs à étiqueter rapidement et précisément les objets dans leur ensemble de données.

Pour choisir le type d'annotation "Label Assists" , cliquez sur le 5ème bouton tout à droite .

![image](https://user-images.githubusercontent.com/123757632/234130382-49faba94-0d50-4751-b640-91d33779f25f.png)

Utiliser les prédictions d'un modèle public ou d'un modèle entraîné par Roboflow Train peut servir de point de départ pour annoter de nouvelles images dans ce dataset. Il suffit de cliquer sur "Continue".

![image](https://user-images.githubusercontent.com/123757632/234130504-795f146e-eac0-472d-9d5a-51b4e70c4dda.png)

Après quelques secondes, la classe "person" sera choisie pour une annotation automatique. Ensuite, "Deselect all" et "person" seront cliqués, suivis de "Select 1 Classes" et "Let's Annotate'.

![image](https://user-images.githubusercontent.com/123757632/234130751-0295b858-3cad-481b-81ff-65d3c7c400f4.png)

Il est à noter que l'annotation a été réalisée automatiquement sur toutes les images.

## 5 . Ajout des images dans le dataset

Maintenant, il ne reste plus qu'à ajouter les images annotées à votre dataset. Pour ce faire, il faut cliquer sur la flèche située à gauche pour revenir au projet, puis cliquer sur "Add 10 images to Dataset", suivi de "Add images".

![image](https://user-images.githubusercontent.com/123757632/234130941-9a69aa98-3dc8-415d-bd66-24b6b89aff29.png)


## 6 . Création d'une nouvelle version du dataset

Enfin, il suffit de cliquer sur "Generate New Version" pour créer une nouvelle version du dataset.

![image](https://user-images.githubusercontent.com/123757632/234131157-b6b2cdd3-f0fa-44aa-bcb8-3bd2f37a217f.png)

La fonctionnalité "generate new version" permet également de cloner des ensembles de données existants, en créant une nouvelle version de l'ensemble de données original avec toutes les annotations et les métadonnées associées.

* **Preprocessing (Prétraitement) :** Le prétraitement est une étape de nettoyage et de préparation des données d'origine avant de les utiliser pour entraîner un modèle de vision par ordinateur.

![image](https://user-images.githubusercontent.com/123757632/234131213-63a2edf5-a0bb-4db7-8c15-7dc49d67ad34.png)

Les paramètres de "Prétraitement" seront laissés par défaut avant de cliquer sur "Continuer".

* **Augmentation :** L'augmentation de données consiste à créer de nouvelles données d'entraînement en appliquant des transformations aléatoires à des images existantes.

![image](https://user-images.githubusercontent.com/123757632/234131387-45401fec-1d2a-4bfb-be4f-e9b876df3ea8.png)




