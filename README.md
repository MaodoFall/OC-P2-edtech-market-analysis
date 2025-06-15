# 📊 Analyse de données de systèmes éducatifs

**Projet 2 – Mastère Spécialisé Data Science – OpenClassrooms**  
**Rôle : Data Scientist**  
**Client : Academy (Startup EdTech)**

---

## 🎯 Objectif du projet

L’objectif de ce projet est d’aider **Academy**, une startup spécialisée dans la formation en ligne pour lycéens et étudiants, à **identifier les pays présentant un fort potentiel pour l’expansion internationale** de ses services.  

Pour cela, j’ai mené une **analyse exploratoire approfondie** des données éducatives fournies par la **Banque Mondiale**.

---

## 🗂️ Jeux de données utilisés

Les données proviennent du portail public de la Banque Mondiale et comprennent 5 fichiers CSV :

| Fichier                | Description |
|------------------------|-------------|
| `EdStatsCountry.csv`   | Informations géographiques et économiques des pays (241 lignes, 32 colonnes) |
| `EdStatsCountry-Series.csv` | Sources et commentaires d’indicateurs |
| `EdStatsData.csv`      | Valeurs d’indicateurs par pays et par année (886 930 lignes, 70 colonnes) |
| `EdStatsFootNote.csv`  | Informations sur les estimations d’indicateurs |
| `EdStatsSeries.csv`    | Description détaillée des indicateurs (3665 lignes) |

👉 Analyse centrée sur : `EdStatsCountry.csv` et `EdStatsData.csv`.

---

## 🧪 Étapes de l'analyse

### 🔍 1. Analyse de la qualité des données
- Détection de doublons : **aucun doublon** de pays.
- Taux de remplissage des indicateurs analysé.
- Intervalle d’années pertinent retenu : **1998 à 2013**.

### 🗃️ 2. Sélection d’indicateurs pertinents
Critères :
- Données démographiques (population)
- Niveau de vie (PIB par habitant)
- Accès aux technologies (utilisation d’Internet)

➡️ Sélection manuelle de **3665 indicateurs → filtrage à 1335 → nettoyage final à 27 pays.**

### 🧭 3. Détermination du potentiel par pays
- Transformation du dataset : pays en lignes, indicateurs en colonnes.
- Normalisation des données (échelle 0–1).
- Critères d’éligibilité :
  - Population > 2 millions
  - PIB par habitant ≥ 80 % du PIB/habitant de la France

➡️ Liste finale de pays à **fort potentiel de clients pour Academy**.

---

## 📌 Résultats clés

- Mise en évidence de **27 pays** ayant un potentiel commercial significatif.
- Indicateurs structurants : **PIB par habitant**, **taux d'accès à Internet**, **croissance démographique**.
- Visualisations permettant de comparer les pays selon plusieurs dimensions.

---

## 🛠️ Compétences mobilisées

- Manipulation de données avec **Pandas**
- Visualisation avec **Matplotlib** et **Seaborn**
- Analyse statistique descriptive
- Nettoyage et transformation de données volumineuses
- Rédaction de notebooks explicatifs (**Jupyter**)

---

## 📁 Livrables

- 📓 Notebook Jupyter d’analyse exploratoire
- 🖥️ Support de présentation

---

## 🚀 Perspectives

Cette étude constitue une **base d’aide à la décision stratégique** pour Academy dans le cadre de son expansion à l’international. Une analyse plus poussée par cluster ou scoring de pays serait une suite logique du projet.

---

## 🙋‍♂️ Réalisé par

**Maodo FALL**  
*Data Scientist*  

---
