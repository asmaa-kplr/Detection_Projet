# Qu'est-ce que la détection d'objets ?

La détection d'objets est une tâche de vision par ordinateur qui consiste à identifier et localiser des objets dans des images ou des vidéos. C'est une partie importante de nombreuses applications, telles que la surveillance, les voitures autonomes ou la robotique. 

L'une des premières tentatives réussies pour résoudre le problème de détection d'objets à l'aide de l'apprentissage en profondeur a été le modèle R-CNN (Régions avec des fonctionnalités CNN), développé par Ross Girshick et son équipe chez Microsoft Research en 2014. Ce modèle utilisait une combinaison d'algorithmes de proposition de région et de réseaux de neurones convolutionnels (CNN) pour détecter et localiser des objets dans des images.

# Qu'est-ce qu'un réseau de neurones convolutionnel ?

Un réseau de neurones convolutionnel (également appelé ConvNet ou CNN) est un type de réseau de neurones à alimentation directe utilisé dans des tâches telles que l'analyse d'images, le traitement du langage naturel et d'autres problèmes complexes de classification d'images.

Il est unique en ce qu'il peut identifier et détecter des motifs à partir d'images et de texte, et leur donner du sens. Nous explorerons cela plus en profondeur plus tard dans l'article. Cependant —

Avant de plonger plus profondément dans ce sujet, prenons du recul et comprenons l'origine du réseau de neurones convolutionnel (CNN).

# Architecture des Réseaux de Neurones Convolutionnels : Un Aperçu

Maintenant, explorons les blocs de construction principaux pour une architecture de réseaux de neurones.

## ConvNet vs Réseaux de Neurones à Alimentation Directe

Un ordinateur voit une image comme une matrice de nombres avec une forme (lignescolonnesnombre de canaux). Toute image du monde réel serait d'au moins 2002003 pixels.

La question est donc : pouvons-nous simplement aplatir l'image en une longue matrice 1D ? "Non"

Les réseaux neuronaux qui acceptent cette longue chaîne de nombres doivent contenir un grand nombre de neurones. Le nombre de poids requis à la première couche cachée sera de 20 000.

Le traitement d'une quantité aussi importante de paramètres nécessite de nombreux neurones et peut conduire à un surapprentissage.

Contrairement aux réseaux de neurones à alimentation directe, les réseaux de neurones convolutionnels examinent une partie de l'image à la fois et avancent de cette manière pour obtenir des informations complètes. Il implique très peu de neurones avec moins de paramètres pour balayer une image entière et apprendre les caractéristiques essentielles.

![image](https://user-images.githubusercontent.com/123757632/235911576-e328ec00-213c-4067-89f2-6c07d5cd7283.png)
