# 🌍 Projet 5 – Dashboard Power BI : Données Géopolitiques & Météorologiques  

## 📌 Contexte  

Ce projet a été mené dans le cadre d’un **atelier pratique Power BI** et vise à démontrer la puissance de l’intégration de données issues de **sources API externes** avec des visualisations interactives.  

L’objectif principal était de concevoir un **rapport dynamique et visuellement attractif** permettant de :  
- Explorer les **caractéristiques géopolitiques des pays** (population, superficie, monnaies, langues, continents, etc.).  
- Intégrer la **météo en temps réel** pour chaque pays grâce à des coordonnées GPS.  
- Combiner ces informations dans une **visualisation cartographique interactive** enrichie par des **infobulles personnalisées**.  

Ce projet illustre des compétences clés en **ETL (Power Query)**, **modélisation relationnelle (DAX)** et **dataviz avancée (Power BI)**.  

---

## ⚙️ Technologies & Sources  

- **Power BI Desktop**  
- **Power Query (M Language)**  
- **DAX** (mesures, sélection dynamique, concaténation de valeurs multiples)  
- **APIs externes utilisées** :  
  - 🌐 [RestCountries](https://restcountries.com/) → informations pays (capitale, population, codes ISO, superficie, langues, monnaies, etc.)  
  - 🌦️ [Open Meteo](https://open-meteo.com/) → météo en temps réel par latitude/longitude  
  - 🏳️ [Flagpedia](https://flagpedia.net) → affichage des drapeaux dynamiques  

---

## 🛠 Étapes du projet  

### 🔹 1. Préparation & Transformation des données (Power Query)  
- Connexion à l’API **RestCountries** et sélection des champs pertinents.  
- Nettoyage et transformation des données (capitale, population, coordonnées GPS, superficie, etc.).  
- Création de **tables de référence relationnelles** (langues, monnaies, continents).  
- Génération d’un **appel API météo dynamique** basé sur latitude/longitude.  
- Ajout des **URLs dynamiques des drapeaux** via Flagpedia.  

### 🔹 2. Modélisation des données  
- Construction d’un **modèle relationnel optimisé** entre table principale et tables de référence.  
- Création d’une table calculée `MetricsTable` pour permettre la **sélection dynamique d’indicateurs** (Population, Superficie, Température, Vitesse du vent).  

### 🔹 3. Visualisation principale  
- Conception d’une **carte choroplèthe mondiale** colorée selon la métrique choisie.  
- Ajout de **filtres interactifs** : Continent, Langue, Météo, Température (avec réglette).  
- Mise en place d’un **sélecteur de métriques dynamiques** (via DAX + SWITCH).  

### 🔹 4. Infobulle personnalisée  
- Création d’une **fiche pays dynamique** affichée au survol :  
  - Données socio-démographiques (capitale, population, superficie, langues, monnaies).  
  - Données météo en temps réel (température, vitesse et direction du vent, code météo).  
  - Ajout d’**images dynamiques** : drapeau + icône météo.  

### 🔹 5. Finalisation  
- Mise en page professionnelle avec palette sombre (#121526, #161C32, #262D45).  
- Vérification du modèle, des filtres et de la cohérence des relations.  
- Préparation à un **rafraîchissement automatique des données météo**.  

---

## 📊 Résultats  

Le rapport Power BI permet :  
✅ D’explorer les pays par **région, langue ou climat**.  
✅ D’afficher la **météo actuelle en temps réel** pour chaque pays.  
✅ De consulter des **infobulles enrichies** incluant drapeau et informations clés.  
✅ De comparer plusieurs **indicateurs dynamiques** (Population, Superficie, Température, Vent).  

---

## 🚀 Valeur ajoutée du projet  

- **Intégration multi-API en temps réel** (données géopolitiques + météo).  
- **Modélisation avancée** avec Power Query & DAX.  
- Expérience complète de bout en bout : **ETL → Modèle → Dataviz → UX avancée**.  
- Exemple concret d’un projet **proche des besoins en entreprise** : données enrichies, mise à jour automatique, storytelling visuel.  

---

## 📸 Aperçu du Dashboard  

<img width="677" height="389" alt="Image du dashbord_geo" src="https://github.com/user-attachments/assets/3db01c7d-c515-458a-9eae-22b4d149cf36" />
 
![image 2 infobule carte](https://github.com/user-attachments/assets/c74aa5cb-4dfa-47e7-85a1-754de1d24737)
  
![Exemple Infobulle](images/infobulle_example.png)  

---

## 📂 Structure du projet  

