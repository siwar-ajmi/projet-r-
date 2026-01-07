# 🏥 Audit Stratégique : Parc de Mammographie en Tunisie 🇹🇳



## 📌 1. Présentation du Projet
Le cancer du sein est le premier cancer féminin en Tunisie. Cet audit technologique du parc hospitalier public vise à répondre à une question de santé publique majeure : **Le réseau public est-il équipé pour un dépistage précoce équitable ?**

Ce projet analyse la **fracture numérique territoriale** en segmentant les équipements par technologie (Numérique vs Conventionnel) et par région, offrant ainsi un outil d'aide à la décision pour les politiques de santé.
[👉 Cliquer ici pour ouvrir le Notebook directement dans Google Colab](https://colab.research.google.com/github/siwar-ajmi/projet-r/blob/main/mammographie.ipynb)---

## 🚀 2. Objectifs et Problématique
1. **Évaluer la Modernisation** : Quelle est la proportion d'appareils numériques (haute précision) face aux anciens modèles conventionnels ?
2. **Analyser la Répartition** : Existe-t-il une inégalité d'accès aux soins entre le Grand Tunis et les régions intérieures ?
3. **Validation Statistique** : Utiliser les mathématiques pour prouver si la distribution est équilibrée ou non.

---

## 🛠️ 3. Méthodologie & Outils
Le projet suit une démarche de Data Science rigoureuse :
* **Nettoyage de données (Wrangling)** : Standardisation des noms de marques (GE, Hologic, Fuji) et création d'une segmentation régionale (Feature Engineering).
* **Visualisation Avancée** : Création d'un Dashboard combinant un *Donut Chart* (technologie) et un *Bar Chart* (géographie).
* **Analyse Statistique** : 
    * **Test de Shapiro-Wilk** pour vérifier la normalité de la distribution.
    * **Régression Linéaire** pour identifier les tendances de dotation.

**Stack Technique :**
* **Langage** : R
* **Librairies** : `tidyverse` (Data), `ggplot2` & `patchwork` (Visualisation), `stats` (Modélisation).
* **Environnement** : Google Colab / R Kernelspec.

---

## 📊 4. Résultats Clés de l'Audit

### 📉 Conclusions Statistiques
* **Distribution Quantitative** : Avec une **p-value de 0.80** au test de Shapiro-Wilk, nous ne pouvons pas rejeter l'hypothèse de normalité. **Le nombre de machines est donc globalement bien réparti par rapport au nombre de régions.**
* **Modèle de Régression** : La tendance montre une stabilité de dotation, confirmant qu'aucune région n'est totalement délaissée en termes de *quantité*.

### ⚠️ Le Défi Technologique
L'audit souligne que la fracture n'est pas quantitative mais **qualitative**. Une partie du parc reste conventionnelle. L'effort d'investissement doit se porter sur le **remplacement technologique** plutôt que sur l'ajout massif de nouvelles unités.



---

## 💡 5. Recommandations Stratégiques
1.  **Modernisation** : Remplacer en priorité les appareils conventionnels dans les zones à forte densité de population.
2.  **Maintenance** : Harmoniser les contrats de maintenance pour garantir un taux de disponibilité maximal.
3.  **Télémédecine** : Exploiter le parc numérique pour instaurer la lecture des clichés à distance (Télémammographie).

---

## 📂 6. Structure du Dépôt
* `README.md` : Présentation générale, méthodologie et résultats de l'audit (ce fichier).
* `mammographie.ipynb` : Notebook complet avec le code source R, les visualisations et les tests statistiques.
* `equipement_mammographie_hopitaux_publics_sans_annee.csv` : Jeu de données source utilisé pour l'analyse.
* `Presentation_Audit.pdf` : Support de présentation visuel (Slides) pour la soutenance orale.
