# Projet de Classification Automatique d'Articles pour "Place de marché"

![Place de marché Logo](place_de_mrche.jpg)

## Description du Projet

Bienvenue dans le repository GitHub du projet pour "Place de marché" ! Il s'agit de réaliser une étude de faisabilité pour automatiser l'attribution des catégories d'articles sur la plateforme e-commerce. Actuellement, les vendeurs attribuent manuellement les catégories, ce qui est peu fiable. Pour rendre l'expérience utilisateur fluide et préparer une future montée en charge, nous cherchons à mettre en place un moteur de classification d'articles basé sur leurs images et descriptions.

## Objectif du Projet

L'objectif principal de ce projet est de développer un moteur de classification d'articles qui attribuera automatiquement des catégories en fonction de leurs images et descriptions. Pour cela, nous allons suivre les étapes suivantes :

1. Prétraitement des données texte ou image selon le cas.
2. Extraction de features à partir des descriptions textuelles et des images.
3. Réduction des features en 2 dimensions pour visualiser les produits sur un graphique 2D.
4. Analyse visuelle pour évaluer la faisabilité de regrouper automatiquement des produits de même catégorie.
5. Calcul de similarité entre les catégories réelles et les catégories issues de la segmentation en clusters pour confirmer notre analyse visuelle.

## Les données 

Les données sur les articles (images et descriptions) sont disponibles [ici](https://s3-eu-west-1.amazonaws.com/static.oc-static.com/prod/courses/files/Parcours_data_scientist/Projet+-+Textimage+DAS+V2/Dataset+projet+pre%CC%81traitement+textes+images.zip)

## Contraintes du Projet

Pour extraire les features texte, nous devrons mettre en œuvre différentes approches de type "bag-of-words" (comptage simple de mots et Tf-idf) ainsi que des approches de type word/sentence embedding avec Word2Vec, Glove, FastText, et USE (Universal Sentence Encoder).

Pour extraire les features des images, nous utiliserons un algorithme de type SIFT / ORB / SURF ainsi qu'un algorithme de type CNN Transfer Learning.
