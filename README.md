# 📊 Sanitoral Project Management Dashboard

Tableau de bord complet de gestion de projets pour **Sanitoral**, incluant l'analyse des données de planification, l'exécution réelle et les performances des livrables.
Sanitoral pilote aujourd’hui de nombreux projets IT et Marketing dans plusieurs régions du monde.
La difficulté n’est pas le manque de données, mais la capacité à identifier rapidement les projets qui nécessitent une attention particulière.
L’objectif de ce tableau de bord est donc de fournir aux directeurs une vision claire, synthétique et actionnable de la performance des projets. »

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

## 📦 Livrable:
[📄 **Tableau de bord**](./Kamoune_Assia_1_Tableau_de_Bord_012026.pbix)

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

**Objectif :** la planification stratégique des produits Sanitoral

**Sections :**
- Propositions de valeur
- Segments de clients
- Canaux de distribution
- Relations clients
- Flux de revenus
- Ressources clés
- Activités principales
- Partenariats clés
- Structure de coûts

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

##  LA LOGIQUE GLOBALE DU TABLEAU DE BORD 
 Le tableau de bord est organisé pour permettre une lecture en trois niveaux :
- une vue globale en haut, 
- une priorisation des actions au centre, 
- et un niveau de détail en bas pour faciliter la prise de décision.
  
---

## VUE GLOBALE – INDICATEURS CLÉS 
En haut de la page, on retrouve les indicateurs clés du portefeuille de projets :
- le nombre de projets en alerte, 
- la dérive budgétaire, 
- la dérive des délais et le respect des livrables.
- Un seuil d’alerte à 15 % a été défini: Dès qu’un indicateur dépasse ce seuil, il apparaît en rouge afin de signaler un risque potentiel.

---

## OÙ AGIR ? – PRIORISATION DES PROBLÈMES 
- La partie centrale du tableau de bord permet d’identifier où concentrer les efforts.
- La carte du monde met en évidence les pays dans lesquels les projets présentent le plus de dérives.
- Les graphiques complémentaires permettent de comparer les performances par pays, par région ou par type de projet, IT ou Marketing.
- 
---

## AGIR CONCRÈTEMENT – PROJETS À RISQUE 
Une table synthétique présente les projets les plus critiques.
Elle se concentre sur les projets identifiés comme ‘À risque’, et met en avant les cinq projets nécessitant une action prioritaire.
Pour chaque projet, les écarts de coûts et de délais sont visibles, ce qui permet aux directeurs de passer rapidement de l’analyse à l’action.

---

##  ADAPTÉ À TOUS LES RÔLES 
Ce tableau de bord est conçu pour être utilisé par le directeur général, les directeurs régionaux et les directeurs pays.
L’ensemble des utilisateurs accède au même rapport, mais peut filtrer les données selon son périmètre grâce aux segments.
Cela évite la multiplication des pages tout en garantissant une information pertinente pour chaque niveau de responsabilité.

---

## VALEUR AJOUTÉE 
Ce tableau de bord permet de suivre l’avancement des projets, d’identifier rapidement les dérives de performance et de faciliter la prise de décision.
Il transforme des données complexes en une vision claire et actionnable, au service du pilotage stratégique des projets chez Sanitoral.
