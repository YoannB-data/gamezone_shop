# Comprendre et optimiser les performances commerciales d'une entreprise d'e-commerce

# Contexte du projet

L'entreprise Gamezone, fondé en 2018, est une entreprise qui vend des produits liés aux jeux vidéos dans le monde entier.
Elle souhaite mieux comprendre les facteurs influençant ses ventes. 

Les léviers et recommandations sont produits à partir des données clés suivantes :
* Analyse des tendances des ventes : Evaluer l'historique des ventes, à la fois au niveau mondial et par région
* Performances des produits : Identifier les produits qui se vendent le mieux et ceux qui se vendent le moins bien
* Succès des outils : Analyser le vente par rapport aux différents outils mis à dispoisition des clients

# Structure des données & Vérifications initiales

Les données de l'entreprise Gamezone sont structurées en 2 tables.
La première contient les données de ventes, elle a X lignes et X colonnes.
La deuxième contient les régions par pays, elle a X lignes et 2 colonnes.

<p align="center">
  <img width="500" height="250" alt="gamezone-db" src="https://github.com/user-attachments/assets/e4d02cca-8f5e-454e-b284-5637ab4b6342" />
</p>

Avant de commencer l'analyse, un ensemble de manipulation ont été effectuées pour le contrôler la qualité des données et les nettoyer. Le code Python utilisé à ces fins est accessible dans le Jupiter Notebook, parties "2. Découverte du dataframe principal df",  "3. Découverte du dataframe df_region" et "4. Data Cleaning".

# Analyse des données

## Aperçu des résultats

Le chiffre d’affaires atteint 6M$ sur la période, porté par une forte croissance de <b>+160% entre 2019 et 2020</b>. 
Trois produits phares – le <b>27in 4K gaming monitor</b>, la <b>Nintendo Switch</b> et la <b>Sony PlayStation 5</b> – représentent l’essentiel des ventes (75%).
La dynamique commerciale est soutenue par des pics saisonniers (avril, septembre, fin d’année), mais connaît des creux en janvier et octobre. 
Les ventes en ligne via l’app et les réseaux sociaux restent <b>marginales (<3,5%)</b>, ce qui ouvre un fort potentiel de croissance digitale. Enfin, les prix moyens sont stables, confirmant que la performance est tirée par les volumes.

## Analyse approfondie

### 1. Performance globale

* Le chiffre d’affaires cumulé atteint <b>6M$ sur la période</b>, avec une trajectoire très dynamique : les ventes mensuelles progressent de <b>100k$ en janvier 2019 à 250k$ en février 2021</b>, soit une croissance soutenue
* La croissance est particulièrement marquée en <b>2020 (+160% vs 2019)</b>, confirmant une forte expansion du marché et une bonne captation de la demande

<p align="center">
	<img width="538" height="291" alt="image" src="https://github.com/user-attachments/assets/e345cb1a-b66a-4a59-af9a-eaa6a6cb9a18" />
</p>

### 2. Produits phares et portefeuille

* Les ventes sont <b>concentrées sur trois produits majeurs</b> : le 27’’ 4K gaming monitor, la PlayStation 5 et la Nintendo Switch, qui représentent la majorité du chiffre d’affaires
* Le 27’’ 4K gaming monitor est de loin le leader du portefeuille avec près de <b>2M$ de ventes</b>, alors que des produits comme le Razer Pro Gaming Headset génèrent des revenus marginaux (800$)
* Depuis début 2020, on observe un <b>changement structurel</b> : la PS5 connaît une <b>explosion des ventes</b>, alors que la Switch ralentit, illustrant un effet de cannibalisation ou de bascule de préférence client

<p align="center">
	<img width="773" height="309" alt="image" src="https://github.com/user-attachments/assets/fb4b51f1-de3b-4fea-95f0-f548b9476097" />
</p>

### 3. Saisonnalité et comportements clients

* Les ventes affichent une <b>cyclicité marquée</b>, avec trois pics récurrents : <b>avril, septembre et la période de fin d’année (novembre-décembre)</b>
* Les mois de <b>janvier et octobre connaissent des baisses significatives</b>, traduisant une demande post-fêtes en janvier et une baisse pré-Noël en octobre
* L’évolution <b>par région montre des patterns homogènes</b>, ce qui indique une saisonnalité mondiale plutôt que locale

### 4. Canaux de vente

* Les canaux digitaux restent <b>faiblement contributifs</b> : l’app mobile ne représente que <b>2,5% des ventes</b>, et les réseaux sociaux à peine <b>1</b>
* Cela reflète une <b>opportunité stratégique</b> : la digitalisation des ventes est encore sous-exploitée et pourrait être un levier majeur de croissance future

<p align="center">
	<img width="460" height="89" alt="image" src="https://github.com/user-attachments/assets/2770354c-1a3e-4c77-ba1a-927abd7e76bc" />
	<img width="445" height="168" alt="image" src="https://github.com/user-attachments/assets/1054b0a6-32db-4d0d-9547-de3028e8795e" />
</p>

### 5. Prix et volumes

* Les prix de vente unitaires sont stables, ce qui signifie que la croissance est <b>tirée par les volumes vendus</b> et non par une hausse tarifaire
* Cela souligne l’importance d’une stratégie de gestion des stocks et d’approvisionnement efficace pour accompagner la demande croissante


# Recommandations

### Équipe Marketing

1. Exploiter la saisonnalité
	* Intensifier les campagnes mars-avril, août-septembre, novembre-décembre (forte demande)
	* Lancer des promos ciblées en janvier et octobre pour lisser les ventes
2. Focus produits stars
	* 80% des ventes viennent de 3 produits (Monitor 4K, PS5, Switch) : Construire les campagnes cross-selling et bundle offers autour de ces produits
3. Renforcer le digital
	* Développer les ventes via l’app et les réseaux sociaux (actuellement <4% du CA) en intensifiant les campagnes ciblées et en optimisant l’expérience utilisateur mobile


### Équipe Financière

1. Pilotage produit
	* Surveiller la concentration produit : 3 articles génèrent la majorité du CA, ce qui représente un risque de dépendance. Diversifier ou sécuriser l’approvisionnement est clé
2. Analyse ROI des canaux
	* Mesurer la rentabilité des campagnes app & social

### Équipe Produit

1. Focus sur les blockbusters
	* Prioriser les best-sellers : mettre l’accent sur le développement et la disponibilité des produits phares (27’’ 4K Monitor, PS5, Switch) qui tirent la croissance
2. Optimiser la gamme
	* Explorer de nouvelles références dans les catégories sous-représentées
	* Analyser la bascule PS5 vs Switch : comprendre le ralentissement des ventes de la Switch pour adapter la stratégie produit et limiter l’effet de cannibalisation
