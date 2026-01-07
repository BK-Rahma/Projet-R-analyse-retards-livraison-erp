# 📊 Analyse des Retards de Livraison dans un Système ERP

## 📝 Description du projet

Ce projet consiste en une analyse statistique et exploratoire des **retards de livraison** dans un système ERP, à partir des **dates prévues (CHD)** et des **dates réelles (CDD)** des commandes.

L’objectif principal est d’identifier :
- l’ampleur des retards,
- les clients, produits et sites les plus problématiques,
- les tendances temporelles,
- et de fournir des **indicateurs d’aide à la décision** pour améliorer la performance logistique.

L’analyse est réalisée en **R**, en s’appuyant sur des méthodes de nettoyage de données, de calcul d’indicateurs, et de visualisation avancée.

---

## 🎯 Objectifs de l’étude

- Identifier et quantifier les retards de livraison
- Calculer des indicateurs clés de performance (KPI)
- Analyser les retards par :
  - client
  - produit
  - site
- Étudier l’évolution temporelle des retards
- Mettre en place un **système d’alertes logistiques**
- Faciliter la prise de décision opérationnelle

---

## 📂 Données utilisées

- **Source** : Système ERP
- **Fichier** : `Colisageautomatique.csv`
- **Séparateur** : `;`

### Principales informations contenues :
- Dates de création, de livraison, prévues (CHD) et réelles (CDD)
- Clients
- Produits
- Sites logistiques

---

## 🛠️ Technologies & Packages R

- **Langage** : R
- **Packages utilisés** :
  - `tidyverse`
  - `dplyr`
  - `ggplot2`
  - `lubridate`
  - `tidyr`

---

## 🔍 Méthodologie

### 1️⃣ Nettoyage des données
- Suppression des colonnes vides
- Suppression des doublons
- Conversion des dates au format `Date`

### 2️⃣ Calcul des indicateurs
- Retard en jours (`CDD - CHD`)
- Variable binaire `est_en_retard`
- Catégorisation des retards :
  - Pas de retard
  - Léger (1–3 jours)
  - Moyen (4–7 jours)
  - Important (>7 jours)

### 3️⃣ Système d’alertes logistiques
- Livré à temps
- Retard confirmé
- En retard non livré
- Livraison prévue

### 4️⃣ Analyses statistiques
- Analyses globales
- Analyses par client
- Analyses par produit
- Analyses par site
- Heatmap Client × Site

### 5️⃣ Analyses temporelles
- Analyse par mois
- Histogrammes en valeur et en pourcentage
- Évolution du retard moyen
- Analyse détaillée par mois

---

## 📈 Visualisations réalisées

- Histogramme des retards / avances
- Boxplot des retards
- Graphiques par client, produit et site
- Heatmap Client × Site
- Évolution mensuelle des retards
- Diagrammes en barres et camemberts

---

## 📌 Résultats clés

- Identification des clients et sites les plus affectés par les retards
- Mise en évidence de retards importants et récurrents
- Détection de tendances saisonnières
- Visualisation claire des performances logistiques

---

## 👩‍💻 Auteur

**Rahma Bouchnak**  

---
