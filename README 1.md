# 📊 Sanitoral Project Management Dashboard

Tableau de bord complet de gestion de projets pour **Sanitoral**, incluant l'analyse des données de planification, l'exécution réelle et les performances des livrables.

---

## 📋 Table des Matières

- [Vue d'ensemble](#vue-densemble)
- [Structure du Projet](#structure-du-projet)
- [Livrables](#livrables)
- [Données](#données)
- [Utilisation](#utilisation)
- [Stack Technologique](#stack-technologique)
- [Auteur](#auteur)

---

## 🎯 Vue d'ensemble

Ce projet propose une analyse exhaustive du portefeuille de projets de **Sanitoral**, couvrant :

- **Planification des projets** : Durée prévue, coûts estimés, livrables attendus
- **Exécution réelle** : Durée effective, coûts réels, livrables livrés
- **Performance** : Écarts de délai, écarts de budget, taux de réussite des livrables
- **Géographie** : Analyse par pays, région et type de partenariat

### Objectifs principaux

✅ Suivi centralisé de tous les projets et leurs phases  
✅ Comparaison Prévu vs Réel pour les délais, coûts et livrables  
✅ Tableau de bord interactif Power BI pour la visualisation  
✅ Dictionnaire des données pour une compréhension claire des métriques  
✅ Canvas stratégique pour la planification produit  

---

## 📁 Structure du Projet

```
sanitoral-project-management/
├── README.md                                 # Ce fichier
├── 📊 Kamoune_Assia_1_Tableau_de_Bord_012026.pbix
│   └── Tableau de bord Power BI interactif avec visualisations
├── 📋 Donneg_es_Sanitoral_1_.xlsx
│   └── Dataset complet avec 7 feuilles de données
├── 📖 Dictionnaire_des_donne_es_2_.xlsx
│   └── Documentation technique des champs et types de données
└── 📝 Mode_le_de_Product_Strategy_Canvas_a__comple_ter.docx
    └── Template du Product Strategy Canvas à compléter
```

---

## 📦 Livrables

### 1. **Tableau de Bord Power BI** 
📊 `Kamoune_Assia_1_Tableau_de_Bord_012026.pbix`

**Contenu :**
- Visualisations interactives des données de projets
- KPIs clés : délais, budgets, livrables
- Filtres par type de projet, pays, région
- Analyse des écarts Prévu vs Réel
- Tendances temporelles des projets

**Prérequis :**
- Microsoft Power BI Desktop ou Power BI Online
- Connexion aux données Sanitoral Excel

---

### 2. **Dataset Complet**
📋 `Donneg_es_Sanitoral_1_.xlsx`

**Feuilles incluses :**

| Feuille | Description |
|---------|-------------|
| **Projects_plans** | Plan initial de chaque projet lancé (durée, coûts, livrables prévus) |
| **Project type** | Classification des types de projets (IT, Marketing, etc.) |
| **Actual_Costs** | Coûts réels constatés par phase |
| **Actual_Duration** | Durées réelles observées par phase |
| **Actual_Delivrable** | Livrables réellement livrés par phase |
| **Projects_Locations** | Localisation géographique des projets |
| **Country_Profiles** | Profils pays avec type de partenariat (Affilié/Distributeur) |

**Format :** Microsoft Excel (.xlsx)  
**Nombre de lignes :** ~999 enregistrements de phases projet  
**Champs clés :** Project ID, Phase, Start Date, Duration, Cost, Deliverables

---

### 3. **Dictionnaire des Données**
📖 `Dictionnaire_des_donne_es_2_.xlsx`

**Contenu :**
- Nom de chaque champ
- Description détaillée du champ
- Type de données (String, Integer, Datetime, etc.)
- Contexte d'utilisation (données estimées vs réelles)

**Champs documentés :**
- Project ID, Project Type, Country, Phase
- Start Date, Actual_Duration, Actual_Cost, Actual_Deliverables
- Planned_Duration, Planned_Cost, Planned_Delivrable
- Region, Type (Affilié/Distributeur)

**Usage :** Consulter avant tout travail d'analyse ou développement

---

### 4. **Product Strategy Canvas**
📝 `Mode_le_de_Product_Strategy_Canvas_a__comple_ter.docx`

**Objectif :** Template pour la planification stratégique des produits Sanitoral

**Sections à compléter :**
- Propositions de valeur
- Segments de clients
- Canaux de distribution
- Relations clients
- Flux de revenus
- Ressources clés
- Activités principales
- Partenariats clés
- Structure de coûts

**Format :** Microsoft Word (.docx) - Éditable

---

## 📊 Données

### Structure des Données

#### Clés primaires
- **Project ID** : Identifiant unique pour chaque projet
- **Phase** : Identifie la phase unique au sein d'un projet

**Note importante :** Chaque ligne représente une **phase de projet** unique, non un projet complet. Un projet peut avoir plusieurs phases (Planning, Initiation, Execution, Closure, etc.).

#### Colonnes principales

**Données estimées (pré-démarrage) :**
- `Planned_Duration` : Jours prévus
- `Planned_Cost` : Coût USD estimé
- `Planned_Delivrable` : Nombre de livrables attendus

**Données réelles (post-phase) :**
- `Actual_Duration` : Jours constatés
- `Actual_Cost` : Coût USD réel
- `Actual_Deliverables` : Livrables effectivement livrés
- `Start Date` : Date de démarrage réelle

**Contexte géographique :**
- `Country` : Pays d'exécution
- `Region` : Région (ex: EMEA, APAC, Americas)
- `Type` : Partenariat (Affilié ou Distributeur)

### Plages de données

- **Période couverte** : 2018-2024
- **Nombre de projets** : +150
- **Nombre de phases** : ~999
- **Pays représentés** : 20+ pays

---

## 🚀 Utilisation

### Pour les analystes métier

1. **Ouvrir le Dashboard Power BI**
   ```
   → Double-cliquer sur Kamoune_Assia_1_Tableau_de_Bord_012026.pbix
   → Sélectionner les filtres désiré (Pays, Type de projet, Période)
   → Analyser les KPIs et les tendances
   ```

2. **Consulter le dictionnaire des données**
   ```
   → Ouvrir Dictionnaire_des_donne_es_2_.xlsx
   → Identifier les champs nécessaires
   → Vérifier les types de données et contextes
   ```

### Pour les développeurs / Data Engineers

1. **Charger les données**
   ```python
   import pandas as pd
   
   # Charger le dataset principal
   df = pd.read_excel('Donneg_es_Sanitoral_1_.xlsx', sheet_name='Projects_plans')
   
   # Consulter la structure
   print(df.info())
   print(df.head())
   ```

2. **Intégration avec des outils BI**
   - Power BI : Connexion directe Excel ou connexion BDD
   - Tableau : Import Excel ou requête SQL
   - Looker Studio : Google Sheets ou API

3. **Analyse Python/R**
   ```python
   # Exemple : Calculer les écarts Prévu vs Réel
   df['Duration_Variance'] = df['Actual_Duration'] - df['Planned_Duration']
   df['Cost_Variance'] = df['Actual_Cost'] - df['Planned_Cost']
   ```

### Planification produit

1. **Utiliser le Strategy Canvas**
   - Télécharger `Mode_le_de_Product_Strategy_Canvas_a__comple_ter.docx`
   - Remplir chaque bloc avec les informations de votre stratégie
   - Partager et collaborer avec l'équipe

---

## 🛠️ Stack Technologique

| Outil | Version | Usage |
|-------|---------|-------|
| **Power BI** | 2025+ | Dashboard interactif et visualisations |
| **Microsoft Excel** | 365 | Stockage et gestion des données |
| **Microsoft Word** | 365 | Documentation et templates |
| **Python** | 3.8+ | Analyse et ETL (optionnel) |
| **Pandas** | 1.5+ | Manipulation de données (optionnel) |

---

## 📈 KPIs Disponibles

### Délais
- 📅 Écart de durée (Réel vs Prévu)
- 📅 Respect des deadlines par phase
- 📅 Tendance des délais par type de projet

### Coûts
- 💰 Écart budgétaire (Réel vs Prévu)
- 💰 Coût moyen par phase
- 💰 ROI par projet

### Livrables
- ✅ Taux de réussite des livrables
- ✅ Nombre de livrables par phase
- ✅ Performance de livraison

### Géographie
- 🌍 Performance par pays
- 🌍 Analyse par région
- 🌍 Comparaison par type de partenariat

---

## 📚 Documentation supplémentaire

### Colonnes du Dataset

**Projects_plans (Planning Data)**
- `Project ID` : Identifiant unique
- `Phase` : Phase du projet
- `Start Date` : Date de démarrage
- `Planned_Duration` : Durée prévue (jours)
- `Planned_Cost` : Coût prévu (USD)
- `Planned_Delivrable` : Livrables prévus

**Actual_Costs, Actual_Duration, Actual_Delivrable**
- Contiennent les données réelles collectées à la fin de chaque phase
- Horodatage de saisie par l'équipe projet

**Country_Profiles**
- Informations contextuelles sur chaque pays
- Type de partenariat : Affilié ou Distributeur

---

## 🤝 Contribution

Ce projet est actuellement en phase de **visualisation et analyse**. Pour contribuer :

1. Vérifier les données dans le dictionnaire
2. Valider les calculs d'écarts et KPIs
3. Proposer de nouvelles visualisations Power BI
4. Améliorer la documentation

---

## 📧 Contact & Support

**Responsable du projet :** Assia Kamoune  
**Dernière mise à jour :** Janvier 2026  
**Version :** 1.0

Pour toute question ou suggestion :
- 📧 Email : [contact@sanitoral.com](mailto:contact@sanitoral.com)
- 💬 Slack : #project-management

---

## 📄 Licence

Ce projet est **propriétaire à Sanitoral**. Tous les livrables et données sont confidentiels.

---

## 🎓 Glossaire

| Terme | Définition |
|-------|-----------|
| **Phase** | Étape d'un projet (Planning, Initiation, Execution, Closure) |
| **Écart** | Différence entre la valeur prévue et la valeur réelle |
| **ROI** | Retour sur investissement (Return on Investment) |
| **Affilié** | Partenaire commercialisant les services sous sa propre marque |
| **Distributeur** | Partenaire revendant les services de Sanitoral |
| **Délivrable** | Livrables tangibles remis aux clients |
| **DXA** | Unité de mesure Microsoft Office (1440 DXA = 1 pouce) |

---

**Merci d'utiliser le tableau de bord Sanitoral !** 🎯
