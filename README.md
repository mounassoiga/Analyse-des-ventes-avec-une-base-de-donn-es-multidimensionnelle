# 📊 Projet BI : Analyse de Performance Commerciale (End-to-End)

## 🌟 Présentation du Projet
Ce projet illustre la mise en place d'une solution décisionnelle complète (Business Intelligence), de la conception du Data Warehouse à la visualisation de données interactive. L'objectif est d'extraire des insights stratégiques à partir de données transactionnelles brutes.

---

## 🏗️ Architecture Technique

### 1. Data Warehouse (SSMS)
* **Modélisation** : Schéma en **Flocon de Neige** (Snowflake).
* **Structure** : 5 tables de dimensions (`Customers`, `Employee`, `Location`, `Products`, `SDate`) reliées à une table de faits (`Fact_Ventes`).
* **Source** : Données extraites de `SalesOrders` et `SalesOrdersDetails`.

### 2. ETL & Intégration (SSIS)
* Création de packages **SSIS** pour l'extraction, la transformation et le chargement (ETL) des données vers le Data Warehouse.
* Automatisation de la collecte des mesures et des clés étrangères.

### 3. Analyse Multidimensionnelle (SSAS)
* Développement d'un **Cube OLAP** sous SQL Server Analysis Services.
* **KPIs calculés** : Marge brute, prix de vente moyen, etc.
* **Hiérarchies** : Mise en place de drill-down pour le temps (Année > Mois) et la géographie (Pays > Ville).

### 4. Dashboard Web (Streamlit & Python)
* Interface utilisateur développée en **Python** avec le framework **Streamlit**.
* Connexion au cube via `pyodbc` / `MSOLAP` pour l'exécution de requêtes **MDX**.
* **Visualisations** : Graphiques de rentabilité, Top 10 clients et indicateurs de performance clés.

---

## 🚀 Installation et Utilisation
1. Clonez ce dépôt : `git clone https://github.com/votre-pseudo/votre-projet.git`
2. Installez les dépendances : `pip install -r requirements.txt`
3. Configurez votre chaîne de connexion dans `dashboard_streamlit.py`.
4. Lancez l'application : `streamlit run dashboard_streamlit.py`

---

## 🛠️ Technologies
* **Base de données** : SQL Server (SSMS)
* **ETL** : SQL Server Integration Services (SSIS)
* **Analyse** : SQL Server Analysis Services (SSAS)
* **Visualisation** : Python / Streamlit
* **Langages** : SQL, MDX, Python

---

**Auteur : Maimouna Abdoulaye oiga , Etudiante en master de sciences et ingénierie des données**
