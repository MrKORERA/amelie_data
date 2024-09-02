1. Description du projet :
Ce projet vise à analyser les données sur le cancer en utilisant une base de données DuckDB. Le script RMarkdown se connecte à la base de données, récupère les données pertinentes, et génère des tableaux descriptifs et résumés statistiques en utilisant les packages gtsummary et flextable. Le rapport final est exporté au format HTML pour une visualisation facile.
2. Étapes :
1.	Chargement des packages :
Les packages nécessaires sont chargés pour permettre la manipulation des données, la connexion à la base de données, et la création des tableaux descriptifs.
2.	Connexion à la base de données :
Le script se connecte à une base de données DuckDB située localement via le chemin spécifié. Cette connexion est nécessaire pour interroger et extraire les données à analyser.
3.	Récupération des données :
Une requête SQL est exécutée pour extraire les données de la table cancer_data dans un DataFrame R.
4.	Analyse des pathologies :
Le script génère un tableau récapitulatif du nombre de cas de pathologies par année, groupé par la variable patho_niv3. Le tableau est formaté pour une présentation soignée à l'aide du package flextable.
5.	Analyse descriptive avec gtsummary :
Un tableau récapitulatif du DataFrame est créé à l'aide de gtsummary, fournissant des statistiques descriptives sur les variables présentes.
6.	Génération du rapport :
Le rapport est compilé et généré au format HTML, incluant tous les tableaux et analyses effectués.
3. Prérequis :
•	R : Le langage R doit être installé sur votre machine. Vous pouvez le télécharger depuis le site officiel de R.
•	RStudio : Il est recommandé d'utiliser RStudio pour exécuter le script RMarkdown. Vous pouvez le télécharger depuis le site officiel de RStudio.
•	Packages R : Assurez-vous que les packages suivants sont installés :
o	dplyr
o	flextable
o	gtsummary
o	DBI
o	duckdb
Vous pouvez installer les packages manquants en exécutant le code suivant dans la console R :
install.packages(c("dplyr", "flextable", "gtsummary", "DBI", "duckdb"))

4. Instructions d'Exécution :
1.	Ouvrir le projet :
o	Clonez ou téléchargez le projet sur votre machine.
o	Ouvrez le fichier .Rmd dans RStudio.
2.	Lancer l'analyse :
o	Avant d'exécuter le fichier RMarkdown, assurez-vous que la base de données DuckDB est accessible à l'emplacement spécifié dans le code et que les packages dplyr, flextable, gtsummary, DBI, duckdb sont installés.
o	Cliquez sur le bouton "Knit" dans RStudio pour compiler le rapport en HTML.
3.	Visualisation du Rapport :
o	Une fois le processus terminé, le rapport HTML sera généré et automatiquement ouvert dans votre navigateur pour visualisation.
