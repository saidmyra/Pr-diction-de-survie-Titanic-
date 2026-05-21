# 🚢 Titanic Survival Prediction

<div align="center">

<img src="https://img.shields.io/badge/Machine%20Learning-Classification-blue?style=for-the-badge" />
<img src="https://img.shields.io/badge/Python-ScikitLearn-yellow?style=for-the-badge" />
<img src="https://img.shields.io/badge/Kaggle-Titanic-red?style=for-the-badge" />
<img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" />

<br><br>

### 📊 Projet Machine Learning — Régression Logistique & Random Forest

Analyse et prédiction de la survie des passagers du Titanic à partir des données Kaggle.

</div>

---

# 📌 Objectif du projet

Ce projet a pour objectif de construire un pipeline complet de Machine Learning capable de prédire si un passager du Titanic a survécu ou non.

Le projet couvre :

✅ Analyse exploratoire des données  
✅ Préparation & nettoyage des données  
✅ Feature Engineering  
✅ Construction de modèles ML  
✅ Évaluation des performances  
✅ Soumission Kaggle  

---

# 🧠 Problématique

> Peut-on construire un pipeline de classification binaire fiable pour prédire la variable `Survived` à partir des données Titanic ?

---

# ⚙️ Technologies utilisées

<div align="center">

| Machine Learning | Data Processing | Visualisation |
|---|---|---|
| Scikit-Learn | Pandas | Matplotlib |
| Logistic Regression | NumPy | Seaborn |
| Random Forest | ColumnTransformer | Confusion Matrix |

</div>

---

# 🗂️ Préparation des données

## 🔹 Variables numériques
- Age
- Fare

## 🔹 Variables catégorielles
- Sex
- Embarked
- Pclass

---

# 🧹 Pipeline de preprocessing

## 📦 Encodage des variables catégorielles

```python
OneHotEncoder()
```

Transformation des catégories en variables exploitables par les modèles ML.

---

## 📏 Normalisation des variables numériques

```python
StandardScaler()
```

Standardisation des données numériques afin d’harmoniser les échelles.

---

## ⚡ Pipeline global

```python
ColumnTransformer()
```

Application automatique des traitements selon le type de variable.

---

# 🧪 Feature Engineering

Le Feature Engineering a permis d’améliorer significativement les performances du modèle.

---

## 👨‍👩‍👧 FamilySize

```python
FamilySize = SibSp + Parch + 1
```

Représente la taille de la famille embarquée.

---

## 👤 IsAlone

```python
IsAlone = FamilySize == 1
```

Indique si le passager voyage seul.

---

## 🎩 Title Extraction

Extraction du titre social :

- Mr
- Mrs
- Miss
- Master
- etc.

👉 Permet d’ajouter une information implicite sur le statut social.

---

# 🤖 Modèles utilisés

## 🔹 Logistic Regression
✔️ Modèle simple  
✔️ Rapide  
✔️ Interprétable  

---

## 🔹 Logistic Regression + Features
Ajout des variables issues du Feature Engineering.

---

## 🌲 Random Forest
Ensemble d’arbres décisionnels permettant une meilleure généralisation.

---

# 📊 Comparaison des performances

| Modèle | Accuracy | ROC-AUC |
|---|---|---|
| Logistic Regression | 0.80 | 0.84 |
| Logistic + Features | 0.84 | 0.88 |
| Random Forest | 0.80 | 0.846 |

---

# 📈 Analyse des résultats

## ✅ Points forts

✔️ Bonne accuracy globale  
✔️ Bonne capacité de discrimination (ROC-AUC)  
✔️ Pipeline ML complet et robuste  
✔️ Feature Engineering très efficace  

---

## ⚠️ Limites

- Présence de valeurs manquantes
- Généralisation limitée à d'autres datasets
- Certains survivants restent non détectés

---

# 🔍 Insights clés

## 🚀 Feature Engineering = énorme impact

Le Feature Engineering améliore fortement les performances :

```python
Accuracy : 0.80 → 0.84
```

---

## 🌲 Random Forest généralise mieux

Même si la régression logistique obtient de bons résultats localement :

- le Random Forest performe mieux sur Kaggle
- il généralise mieux sur des données inconnues

---

# 🏆 Conclusion

## ✅ Ce projet montre :

- l’importance du preprocessing
- l’impact du Feature Engineering
- la différence entre performance locale et généralisation réelle

👉 Le modèle **Random Forest** est finalement retenu comme meilleur modèle global.

---

# 📂 Structure du projet

```bash
📦 titanic-ml-project
 ┣ 📂 data
 ┣ 📂 notebooks
 ┣ 📂 models
 ┣ 📂 outputs
 ┣ 📜 train.py
 ┣ 📜 predict.py
 ┣ 📜 requirements.txt
 ┗ 📜 README.md
```

---

# ▶️ Installation

```bash
git clone https://github.com/your-username/titanic-ml-project.git
cd titanic-ml-project
pip install -r requirements.txt
```

---

# 🚀 Lancement du projet

```bash
python train.py
```

---

# 👨‍💻 Auteurs

- Said Myra

---

# 🌟 Aperçu

<div align="center">

🚢 Machine Learning • Kaggle • Classification • Scikit-Learn

</div>
