# YOLO
En un seul passage, la famille de modèles de vision par ordinateur YOLO (You Only Look Once) utilise un réseau de neurones pour prédire la position des rectangles englobants et les probabilités de classification d'une image. En d'autres termes, il s'agit d'une méthode permettant d'identifier et de reconnaître des objets dans des photographies en temps réel.

Le modèle est devenu largement connu après que ses développeurs, Joseph Redmon, Santosh Divvala, Ross Girshik et Ali Farhadi, ont présenté la nouvelle architecture lors de la Conférence CVPR sur la vision par ordinateur et la reconnaissance de formes en 2016, et ont même remporté le prix OpenCV People Choice Awards pour cela.

**Mais d'où vient YOLO, quelle est sa nouveauté et pourquoi y a-t-il tant de versions ?**

Le YOLO (You Only Look Once) original a été écrit par Joseph Redmon dans un framework personnalisé appelé Darknet.

Darknet est un framework de recherche très flexible écrit en langages de bas niveau qui a produit une série des meilleurs détecteurs d'objets en temps réel en vision par ordinateur : YOLO, YOLOv2, YOLOv3, YOLOv4, YOLOv5, YOLOV6 et maintenant YOLOV7.

![image](https://user-images.githubusercontent.com/123757632/233953603-167b62b9-d741-43eb-8918-deb5674aa126.png)

YOLO a été le premier réseau de détection d'objets à combiner la tâche de dessin de boîtes englobantes et d'identification de libellé de classe en un seul réseau différentiable de bout en bout.

## YOLOv1

Le modèle YOLO de base prédit des images à 45 images par seconde (FPS) sur un GPU Titan X. Les auteurs ont également développé une version beaucoup plus légère de YOLO appelée Fast YOLO, qui a moins de couches et qui traite les images à 155 images par seconde.

Ainsi, YOLO a atteint une précision moyenne de 63,4 mAP (moyenne de précision), plus du double de celle des autres détecteurs en temps réel, ce qui le rend encore plus spécial. Tant YOLO que Fast YOLO surpassent de loin les variantes de détecteurs d'objets en temps réel DPM en termes de précision moyenne (presque deux fois plus) et de FPS.


## YOLOv2

Après sa première introduction en 2016, la famille de modèles YOLO continue d'évoluer chaque année. Par exemple, l'année suivante, le YOLOv2 a été publié. Un certain nombre d'améliorations itératives ont été apportées à l'architecture de YOLO, notamment BatchNorm, une résolution plus élevée et des boîtes d'ancrage.

**BatchNorm est une méthode utilisée pour rendre l'entraînement des réseaux neuronaux artificiels plus rapide et plus stable en normalisant les entrées des couches par recentrage et rescaling.**

À une résolution de données d'entrée de 416x416, YOLOv2 a atteint une précision moyenne de 76,8 mAP sur l'ensemble de données VOC 2007 et 67 FPS sur le GPU Titan X. Sur le même ensemble de données de résolution 544x544, YOLOv2 a atteint une précision moyenne de 78,6 mAP et 40 FPS.

## YOLOv3

En 2018, les développeurs Redmon et Farhadi ont publié YOLOv3, qui s'appuie sur les modèles précédents en ajoutant une estimation de l'objectivité aux prédictions de boîte englobante, en ajoutant des connexions aux couches du réseau de référence, et en effectuant des prédictions à trois niveaux de détail distincts pour améliorer les performances sur les petits objets.

Il est entraîné sur différentes résolutions d'image telles que 320×320, 416×416. À une résolution de 320×320, YOLOv3 atteint une précision moyenne de 28,2 mAP à 45 FPS sur un GPU Titan X et a la même précision que le détecteur à prise de vue unique (SSD321), mais 3 fois plus rapide.
