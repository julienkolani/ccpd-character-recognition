# CCPD Character Recognition

Pipeline de reconnaissance de caractères de plaques d'immatriculation sur le dataset CCPD, sans deep learning.

## Présentation

Approche par correspondance de profils : extraction de primitives basées sur la distance aux bords (gauche/droite), apprentissage par centroïdes K-means comme templates de classe, classification par distance euclidienne avec conversion softmax.

## Résultats

- Jeu de données : CCPD (Chinese City Parking Dataset)
- Jeu de test : ~475 images
- Précision : **81,47%** sur les caractères alphanumériques (0-9, A-Z)

## Stack technique

- Python, OpenCV, NumPy, scikit-learn (K-means)

## Installation

```bash
pip install opencv-python numpy scikit-learn matplotlib
jupyter notebook
```

## Données

Le dataset CCPD n'est pas inclus. À télécharger séparément et à placer dans `data/`.
