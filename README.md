## 📊 Aperçu du projet

Ce notebook Jupyter réalise une **analyse exploratoire des données (EDA)** du dataset **Big Mart Sales**, qui contient les ventes de produits dans différents points de vente Big Mart.

### 🎯 Objectifs

- Nettoyer et préparer les données pour l'analyse
- Identifier les valeurs manquantes et les traiter de manière appropriée
- Analyser les ventes selon différentes dimensions (année, type de magasin, taille, localisation, catégorie de produit)
- Visualiser les tendances et les performances commerciales

### 📁 Structure du notebook

| Étape | Description |
|-------|-------------|
| 1 | Importation des librairies (Pandas, NumPy, Matplotlib, Seaborn) |
| 2 | Chargement et découverte du dataset |
| 3 | Nettoyage : valeurs manquantes sur `Item_Weight` et `Outlet_Size` |
| 4 | Transformation : conversion de l'année en format période |
| 5 | Statistiques descriptives globales |
| 6 | Visualisations thématiques |
| 7 | Export des données nettoyées |

### 🔧 Traitements effectués

| Colonne | Problème | Solution appliquée |
|---------|----------|---------------------|
| `Item_Weight` | 1463 valeurs manquantes | Remplacement par `moyenne - écart-type` |
| `Outlet_Size` | 2410 valeurs manquantes | Remplacement par la valeur la plus fréquente (`Medium`) |
| `Outlet_Establishment_Year` | Type `int` | Conversion en format période annuelle |

### 📈 Visualisations générées

1. **Ventes par année d'établissement**  
   → Barplot montrant l'évolution du chiffre d'affaires selon l'ouverture des magasins

2. **Ventes par type de magasin**  
   → Comparaison entre Grocery Store, Supermarket Type1, Type2 et Type3

3. **Ventes par taille et localisation**  
   → Graphique groupé (hue) croisant `Outlet_Size` et `Outlet_Location_Type`

4. **Moyenne des ventes par type d'article**  
   → Classement des 16 catégories de produits par performance moyenne

### 📌 Résultats clés

- **Supermarket Type1** génère les meilleures ventes (≈13M)
- Les années **2004, 1999 et 2007** sont les plus performantes
- La combinaison **Medium + Tier 3** est la plus rentable
- **Starchy Foods** et **Seafood** ont les meilleures ventes moyennes par article

### 🛠️ Technologies utilisées
### **Python**  pour le nettoyage la manipulation et analyse des données
### *power BI*   pour la visualisation
