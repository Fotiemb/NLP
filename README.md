# NLP

## Titre : Détection de Malwares par Classification Supervisée

### Introduction

Ce projet vise à développer un modèle de détection de malwares basé sur une approche de classification supervisée en utilisant une base de données contenant des caractéristiques extraites de fichiers exécutables. La base de données comprend 138,047 échantillons avec 57 caractéristiques pour chaque échantillon. L'objectif principal est de construire et entraîner un réseau de neurones capable de classifier les fichiers exécutables comme légitimes ou malveillants.

### Difficultés
Nous n'avons pas eu un dataset avec énormément de données pour la mise en place de notre réseau de neurones.

### Exploration de la Base de Données

La base de données comprend des informations telles que la taille du code, la version du linker, la taille des sections, la présence d'imports, la distribution d'entropie des sections, et d'autres caractéristiques pertinentes. Il y a 96,724 fichiers légitimes et 41,323 fichiers malveillants dans la base de données.

### Analyse Statistique

Une analyse statistique a été effectuée sur les caractéristiques pour mieux comprendre la distribution des données. Cela a permis d'identifier des tendances, des corrélations et des caractéristiques importantes pour la classification.

### Prétraitement des Données

Le prétraitement des données a inclus la suppression de caractéristiques inutiles.

### Construction et Entraînement du Modèle

Un réseau de neurones a été construit en utilisant des bibliothèques comme TensorFlow et PyTorch. Le modèle a été configuré avec une architecture appropriée pour la tâche de classification. L'ensemble de données a été divisé en ensembles d'entraînement et de test pour évaluer les performances du modèle.

### Évaluation du Modèle

Le modèle a été évalué en utilisant des métriques telles que la précision, le rappel, et la F1-score et l'AUC.

**Précision**
La précision (précision) est une mesure de la qualité des prédictions positives d'un modèle. Elle est définie comme le nombre de vrais positifs (observations correctement prédites comme positives) divisé par le total des observations prédites comme positives (vrais positifs + faux positifs). En d'autres termes, c'est la capacité du modèle à ne pas attribuer à tort une classe positive à des observations qui ne le sont pas vraiment.

**Rappel (Recall)**
 Le rappel mesure la capacité du modèle à détecter toutes les instances réellement anormales dans le jeu de données. Un rappel élevé signifie que le modèle est sensible à la détection d'anomalies.
 
**F1-Score** 
Le F1-score est la moyenne harmonique entre la précision et le rappel. Il fournit un équilibre entre ces deux métriques. Un F1-score élevé indique un équilibre optimal entre précision et rappel.

**Aire sous la Courbe ROC (AUC-ROC)** 
    
 L'AUC-ROC mesure la capacité du modèle à discriminer entre les instances normales et anormales. Une valeur proche de 1 indique une bonne performance, tandis qu'une valeur proche de 0.5 suggère une performance aléatoire.

### Conclusion

Ce projet a abouti à la création d'un modèle de détection de malwares basé sur une classification supervisée.
