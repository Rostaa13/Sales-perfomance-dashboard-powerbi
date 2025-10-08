# 💼 Power BI Sales Performance Dashboard

📊 **Type de projet :** Mission freelance – Data Analysis & Business Intelligence  
💡 **Objectif :** Concevoir un tableau de bord Power BI professionnel pour le suivi des ventes, du chiffre d’affaires et des performances commerciales d’une entreprise cliente (confidentiel), à partir de données simulées mais structurées comme dans un cas réel.

---

## 🧭 Contexte du projet

Ce projet a été réalisé dans le cadre d’une **mission freelance**, dans le but de démontrer mes compétences professionnelles en **data cleaning**, **modélisation**, **visualisation** et **analyse de performance commerciale**.  

Bien que les données utilisées soient **fictives**, le projet a été mené selon les **standards réels d’une mission en entreprise**, avec une approche orientée livrable client.  
Le modèle et le tableau de bord ont été conçus comme s’ils étaient destinés à une grande organisation (type **AXA**, **Air France**, ou **Alten**), nécessitant un reporting clair, fiable et visuellement cohérent.

---

## ⚙️ Étapes de réalisation

### 1️⃣ Préparation et traitement des données
- Import du fichier `sales_2.csv` dans **Power Query**  
- Analyse de la **qualité, distribution et profil des colonnes**  
- Application des bons types de données et renommage explicite  
- Création de tables de référence : **Clients, Produits, Régions, Ventes**  
- Suppression des doublons et vérification d’anomalies

### 2️⃣ Validation et contrôle via SQL
- Utilisation de **requêtes SQL** pour valider la cohérence des chiffres du modèle (ventes totales, agrégations régionales et produits)  
- Vérification des totaux et des moyennes par produit/région  
- Contrôle croisé entre les résultats SQL et les mesures DAX Power BI

### 3️⃣ Modélisation des données
- Conception d’un **modèle en étoile (Star Schema)**  
- Relations entre tables par clés primaires et étrangères  
- Vérification manuelle de la direction des relations et de la granularité  
- Création d’une table de mesures centralisée pour les KPI

### 4️⃣ Création des mesures DAX
- `Total ventes = SUM(Ventes[Prix total])`  
- `Nombre de commandes = DISTINCTCOUNT(Ventes[Id commande])`  
- `Quantité vendue = SUM(Ventes[Quantité])`  
- `Commande moyenne = DIVIDE([Total ventes], [Nombre de commandes])`  
- `Taux d’annulation = DIVIDE([Commandes annulées], [Nombre de commandes])`

### 5️⃣ Conception et visualisation Power BI
- Thème visuel professionnel : **Storm (JSON personnalisé)**  
- Couleurs : fond clair (#80AAFF), blocs visuels (#2A71FF)  
- Création de deux onglets :
  1. **Suivi global des ventes**
  2. **Analyse des commandes annulées**
- Intégration de filtres dynamiques (période, région, statut)
- Mise en place d’info-bulles (tooltips) contextuelles et navigation par icônes


---

## 🛠️ Outils & technologies utilisés

| Outil / Langage | Rôle |
|------------------|------|
| **Power BI Desktop** | Création du rapport et visualisation |
| **Power Query** | Nettoyage et transformation des données |
| **SQL** | Vérification de la cohérence et validation des agrégations |
| **DAX (Data Analysis Expressions)** | Calculs des KPI et indicateurs |
| **Data Modeling (Star Schema)** | Structuration logique des données |
| **Excel / CSV** | Source initiale du jeu de données |

---

## 📊 Fonctionnalités clés

- Indicateurs dynamiques : chiffre d’affaires, commandes, taux d’annulation  
- Répartition du CA (chiffres affaires) par région, catégorie et produit  
- Analyse temporelle et suivi de la performance commerciale  
- Tableau interactif des ventes détaillées  
- Info-bulles et filtres multi-niveaux  
- Design clair, moderne et adapté à un usage exécutif

---

## 📸 Aperçu du dashboard

**Page principale – Suivi global des ventes :**  
![Dashboard Overview](./Images/Page_principal_suivi_ventes.png)

**Page secondaire – Commandes annulées :**  
![Cancelled Orders](./Images/Page_secondaire_Commande_annulées.png)

---

## 🧩 Schéma du modèle de données

- Clients (Id client, Nom client)
- Produits (Id produit, Nom produit, Catégorie)
- Régions (Id région, Nom région)
- Ventes (Id commande, Date, Quantité, Prix total, Statut commande, Id client, Id produit, Id région)

---

## 🔍 Comment visualiser le rapport

1. Télécharger le fichier [`rapport_ventes.pbix`](./Rapport/rapport_ventes.pbix)  
2. Ouvrir le fichier avec **Power BI Desktop**  
3. Explorer les différentes pages et filtres interactifs du rapport  

---

## 💡 Résultats et apprentissages

- Conception d’un **projet complet de bout en bout**, de la préparation à la visualisation.  
- Validation des données et cohérence des indicateurs grâce à SQL.  
- Maîtrise du **langage DAX** et du **modèle relationnel** pour la performance des mesures.  
- Application des bonnes pratiques de **data storytelling et design BI professionnel**.  
- Démonstration de ma capacité à mener **un projet freelance de manière autonome**.

---

## 👤 Auteur

**Taha Rostoume**  
📍 *Data Analyst junior | Business Intelligence & Reporting*  
📧 taharostom@yahoo.ca 
🔗 [[LinkedIn](https://www.linkedin.com/in/taha-rostoume/)]
🔗 [GitHub](https://github.com/Rostaa13)

---

## 🏷️ Mots-clés
`Freelance` `Power BI` `SQL` `DAX` `Data Analysis` `Dashboard` `Data Modeling` `Business Intelligence`
