# Introduction
Projet de MLOps Machine learning end to end allant du dataset ( interpretation, pre processing, analyse) en passant par le développement jusqu'au déployement avec une notion d'explicabilité nécessaire dans notre cas d'étude à savoir l'imagerie médicale. Notre dataset est composé d'images médicales cérébrales à classifier grâce au machine learning. Deux algorithmes basés sur la méthode transformer sont proposés : transformer + heatmap ou transformer + attention rollout.

# Le projet
Projet de MLOps Machine learning end to end allant du dataset ( interpretation, pre processing, analyse) en passant par le développement jusqu'au déployement avec une notion d'explicabilité nécessaire dans notre cas d'étude à savoir l'imagerie médicale. Notre dataset est composé d'images médicales cérébrales à classifier grâce au machine learning. Deux algorithmes basés sur la méthode transformer sont proposés : transformer + heatmap ou transformer + attention rollout.

# Qu'est ce que transformers?
Les algorithmes de Transformer avec déploiement d'attention ou cartes thermiques sont des techniques pour visualiser et comprendre comment un modèle de vision Transformer fait des prédictions. Ils peuvent être utiles pour améliorer la transparence et la compréhension des modèles de vision, ce qui peut être important dans des domaines tels que la médecine où les décisions du modèle peuvent avoir des conséquences importantes pour les patients.
Les algorithmes de Transformer avec déploiement d'attention permettent de visualiser les régions de l'image qui ont été les plus influentes pour une prédiction donnée. Cela peut aider à comprendre comment le modèle interagit avec les différentes parties de l'image pour faire des prédictions. Les algorithmes de cartes thermiques fonctionnent de manière similaire, en utilisant une représentation visuelle pour montrer les régions de l'image qui ont été les plus importantes pour une prédiction.
Dans le cas d'un projet de classification de tumeurs cérébrales à l'aide d'un modèle de Vision Transformer, ces algorithmes pourraient être utiles pour comprendre comment le modèle fait des prédictions pour différents types de tumeurs et comment il utilise les informations de l'image pour faire des prédictions. Cela peut aider à identifier des domaines où le modèle peut être amélioré ou des sources potentielles de biais, ce qui peut améliorer la qualité et la fiabilité des résultats.

# Notion d'Explicabilité
L'explicabilité en intelligence artificielle (AI) est la capacité de comprendre et de décrire les décisions et les prédictions d'un modèle de AI. Dans le cas d'un projet de classification de tumeurs cérébrales à l'aide d'un modèle de Vision Transformer, l'explicabilité est importante car les décisions du modèle peuvent avoir des conséquences importantes pour les patients. Il est donc important de comprendre comment le modèle fait des prédictions et de s'assurer que les décisions sont fiables et valides.

L'utilisation de l'explicabilité en AI peut aider à garantir la qualité et la fiabilité des résultats du modèle de Vision Transformer en permettant de comprendre les décisions du modèle et de les valider. Par exemple, en utilisant les algorithmes de déploiement d'attention ou de cartes thermiques décrits précédemment, il est possible de visualiser les régions de l'image qui ont été les plus influentes pour une prédiction donnée, ce qui peut aider à comprendre comment le modèle utilise les informations de l'image pour faire des prédictions.

En outre, l'explicabilité peut également aider à détecter des sources potentielles de biais dans les données ou le modèle, ce qui peut améliorer la qualité et la fiabilité des résultats du modèle. En utilisant l'explicabilité en AI dans ce projet, il est possible d'améliorer la transparence et la compréhension des décisions du modèle de Vision Transformer, ce qui peut aider à garantir que les résultats sont fiables et valides pour la classification de tumeurs cérébrales.

# A propos du dataset 
Source : https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri
Le dataset "Brain Tumor Classification MRI" disponible sur Kaggle comprend des images d'IRM du cerveau étiquetées pour indiquer si elles contiennent ou non une tumeur. Les données sont organisées en deux dossiers: "yes" et "no" qui contiennent respectivement 253 et 98 images d'IRM de cerveau.

En tant que data analyst, il est important de comprendre les caractéristiques de ce dataset pour pouvoir en tirer le meilleur parti pour notre analyse.

Distribution des classes: Les données sont assez déséquilibrées avec un ratio de 2,6 : 1 entre les images avec une tumeur et sans tumeur. Cela peut avoir une influence sur la précision de la modélisation, il est donc important de s'assurer que la méthode choisie tienne compte de cet écart de distribution.
Qualité et taille des images: Il est important de vérifier la qualité des images et la résolution pour s'assurer qu'elle est suffisante pour notre analyse. Les images d'IRM ont généralement une résolution assez élevée et un niveau de détail important, ce qui peut nécessiter une puissance de calcul supplémentaire pour traiter les données.
Annotation des données: Il est important de vérifier la qualité de l'annotation des données pour s'assurer que les étiquettes sont correctes et cohérentes. Les erreurs dans les annotations peuvent affecter les résultats de la modélisation.
En conclusion, le dataset "Brain Tumor Classification MRI" est un ensemble de données intéressant pour l'analyse en imagerie médicale. Les images d'IRM fournissent un niveau de détail important et la distribution des classes peut représenter un défi pour la modélisation. Il est important de vérifier la qualité et la cohérence des données pour garantir des résultats précis et fiables.

# Choix du modèle d'apprentissage

Keras et scikit-learn (Sklearn) sont tous deux des bibliothèques populaires pour le développement de modèles d'apprentissage automatique en Python. Toutefois, ils ont des objectifs différents et des fonctionnalités spécifiques qui les rendent plus appropriés pour certaines tâches.

Keras est une bibliothèque d'apprentissage profond qui se concentre sur la simplification du développement de réseaux de neurones complexes. Il fournit une interface haut niveau pour construire, former et évaluer des modèles d'apprentissage profond en utilisant des couches prédéfinies et des algorithmes optimiseurs. Cela en fait un choix populaire pour les projets de reconnaissance d'images, de traitement du langage naturel et de génération de contenu.

D'un autre côté, Sklearn est une bibliothèque pour les algorithmes d'apprentissage supervisé et non supervisé. Il offre un large éventail d'algorithmes, tels que les régressions, les arbres de décision, les k-means, etc. avec une interface cohérente et simple à utiliser. Sklearn est souvent utilisé pour les projets de classification, de régression et de clustering.

En résumé, Keras peut être un choix plus approprié pour les projets d'apprentissage profond tels que la classification
