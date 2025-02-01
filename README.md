# Détection de Fraudes - Méthode à Deux Niveaux

Ce projet implémente une **méthode à deux niveaux** pour la détection de fraudes dans les transactions financières. L'approche combine l'**apprentissage supervisé (Régression Logistique)** et l'**apprentissage non supervisé (clustering K-Means)** afin d'améliorer la précision de la détection des fraudes.

## Méthodologie

### Niveau 1 : Régression Logistique
Au premier niveau, un modèle **de régression logistique** est entraîné sur des données étiquetées pour classer les transactions comme **frauduleuses (1)** ou **normales (0)**.

### Niveau 2 : Clustering K-Means
Après avoir identifié les transactions suspectes grâce à la régression logistique, le **clustering K-Means** est appliqué pour segmenter ces transactions en :
- **Fraudes potentielles** (transactions frauduleuses)
- **Non-fraudes** (fausses alertes)

Ce processus en deux étapes permet de réduire le bruit et d'améliorer la précision du système de détection de fraudes.

## Dataset

Le dataset utilisé dans ce projet est disponible au lien suivant :  
[Dataset pour la Détection de Fraudes](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)  

Ce dataset contient des transactions réelles, y compris des transactions frauduleuses, et est utilisé pour entraîner et évaluer les modèles.

## Installation

1. Clone ce repository :
    ```bash
    git clone https://github.com/ton-nom-utilisateur/fraud-detection-two-levels.git
    cd fraud-detection-two-levels
    ```



