# 🚀 Analyse des Propriétés des Alliages avec les Réseaux de Neurones Graphiques (GNN) ⚙️

## 🌟 Présentation du Projet
Ce projet propose le développement d'un modèle de Réseau de Neurones Graphiques (GNN) dédié à l'analyse des propriétés des alliages ternaires. L'objectif principal est de prédire les configurations atomiques avec précision tout en réduisant le coût computationnel des simulations traditionnelles.

Les alliages présentent des structures complexes qui rendent difficile la modélisation de leurs propriétés. Grâce à l'approche GNN, il devient possible de représenter ces structures sous forme de graphes, où chaque atome est un nœud et chaque liaison entre atomes est une arête. Cette représentation permet au modèle d'apprendre les relations spatiales entre les atomes et de fournir des prédictions fines des propriétés des matériaux.

## 📌 Démarche
1. 🔍 **Préparation des Données** :
   - Lecture du fichier `data2.csv` contenant les coordonnées spatiales (X, Y, Z) et les valeurs d'énergie des atomes.
   - Calcul des distances entre chaque paire d'atomes pour construire la matrice de distances.
2. 📐 **Construction du Graphe** :
   - Création des arêtes du graphe en fonction d'un seuil de distance.
   - Conversion des données en un format compatible avec PyTorch Geometric.
3. 🏗️ **Conception du Modèle** :
   - Conception d'un GNN avec trois couches convolutionnelles (GCNConv) et une couche complètement connectée.
4. 📊 **Entraînement et Évaluation** :
   - Division des données en ensembles d'entraînement, de validation et de test.
   - Entraînement du modèle sur 100 époques en utilisant l'erreur absolue moyenne (MAE) comme métrique de performance.
5. 🌐 **Visualisation** :
   - Représentation graphique des interactions atomiques pour visualiser les relations entre atomes et identifier les nœuds clés.

## 🏆 Résultats
Le modèle a démontré une grande précision avec des valeurs de MAE faibles et stables : environ 0,707 pour l'entraînement et 0,713 pour la validation. Ces résultats mettent en évidence la capacité du GNN à apprendre les relations atomiques complexes sans sur-apprentissage. Les visualisations générées offrent un aperçu clair de la structure atomique et des connexions significatives entre les atomes.

## 🚀 Utilisation
Pour utiliser ce projet, suivez les étapes ci-dessous :

1. 📥 **Cloner le projet** :
   ```bash
   git clone https://github.com/yourusername/gnn-alloy-analysis.git
   cd gnn-alloy-analysis
   ```

2. 📌 **Lancer le Notebook** :
   ```bash
   jupyter notebook projet_scientifique.ipynb
   ```

## 🛠️ Technologies Utilisées
- Python
- PyTorch Geometric
- Pandas, NumPy, SciPy
- NetworkX, Matplotlib

## 📈 Perspectives
Ce projet ouvre la voie à des améliorations futures, telles que l'optimisation des hyperparamètres et l'exploration de nouvelles architectures GNN pour affiner davantage les prédictions.



---
Projet développé dans le cadre d'un projet scientifique à l'École Centrale de Casablanca.

