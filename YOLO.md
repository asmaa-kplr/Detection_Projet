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

![image](https://user-images.githubusercontent.com/123757632/233956870-191ccd75-ce51-445a-abdb-30e1b7e4ba04.png)

