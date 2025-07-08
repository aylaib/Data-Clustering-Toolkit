# Application d'Analyse et de Clustering de Données

Ce projet, développé en Python avec Jupyter et Tkinter, est une application complète pour l'exploration de données et l'application de divers algorithmes de clustering. Il a été réalisé dans le cadre du module de Fouille de Données (M1 Bio-Informatique, USTHB).

L'application offre une interface graphique intuitive permettant de réaliser un pipeline complet de data mining, du prétraitement à l'évaluation des performances des clusters.

## 📸 Captures d'écran

![Interface Principale de l'Application](screenshots/app.png)
_Interface principale de l'application offrant des outils de prétraitement et de clustering._

![Courbe d'Elbow pour K-Means](screenshots/elbow_curve.png)
_Exemple de la méthode du coude (Elbow) pour déterminer le nombre optimal de clusters._

## ✨ Fonctionnalités

### 1. Prétraitement et Analyse Exploratoire (EDA)
- **Chargement de Données :** Ouverture de fichiers `.csv` et `.arff`.
- **Exploration :** Affichage des valeurs distinctes, nombre d'instances, informations sur les attributs.
- **Statistiques Descriptives :** Calcul du Min, Max, Moyenne, Médiane et Quartiles.
- **Visualisation :** Génération de **Boxplots** et **Scatter plots** pour analyser les distributions et corrélations.
- **Nettoyage :** Détection et remplacement des valeurs manquantes.
- **Normalisation :** Mise à l'échelle des données via les méthodes **Min/Max** et **Z-score**.

### 2. Algorithmes de Clustering
L'application implémente et compare 5 algorithmes de clustering majeurs :
- **K-Means :** Basé sur les centroïdes.
- **K-Medoids :** Variante robuste utilisant des médoïdes.
- **AGNES (Agglomerative Nesting) :** Clustering hiérarchique ascendant.
- **DIANA (Divisive Analysis) :** Clustering hiérarchique descendant.
- **DBSCAN (Density-Based) :** Clustering basé sur la densité, capable de trouver des formes arbitraires.

### 3. Évaluation des Performances
- **Méthode du Coude (Elbow) :** Pour déterminer le nombre optimal de clusters (k).
- **Mesures d'Inertie :** Calcul de l'inertie intra-classe et inter-classe.
- **Scores de Clustering :** Évaluation via le **Score de Silhouette**, l'**Indice de Calinski-Harabasz** et l'**Indice de Davies-Bouldin**.

## 🛠️ Technologies et Bibliothèques

- **Python 3**
- **Tkinter** pour l'interface graphique (GUI)
- **Jupyter Notebook** pour l'environnement de développement
- **Pandas** & **Numpy** pour la manipulation des données
- **Scikit-learn** & **Scikit-learn-extra** pour les algorithmes de clustering et le prétraitement
- **Matplotlib** & **Seaborn** pour la visualisation des données
- **Kneed** pour l'analyse de la courbe d'Elbow

## 🚀 Comment l'utiliser

1.  **Clonez le dépôt :**
    ```bash
    git clone https://github.com/VOTRE_NOM_UTILISATEUR/Data-Clustering-Toolkit.git
    cd Data-Clustering-Toolkit
    ```

2.  **Installez les dépendances :**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Lancez Jupyter Notebook :**
    ```bash
    jupyter notebook
    ```

4.  Dans l'interface de Jupyter, naviguez dans le dossier `notebook/` et ouvrez `Clustering_Analysis.ipynb`.

5.  Exécutez les cellules du notebook. La dernière cellule lancera l'application graphique Tkinter.

## 📚 Documents de Référence
- **[Rapport Complet du Projet](./Rapport_Projet_Clustering.pdf)** : Analyse détaillée, méthodologie, résultats et conclusions.