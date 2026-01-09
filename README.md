1. Objectif du projet Démontrer si un portefeuille construit sur des critères subjectifs (centres d'intérêt) peut générer un surplus de rentabilité par rapport à un investissement passif diversifié, tout en mesurant précisément le risque systématique encouru.

2. Méthodologie & Programmation

Extraction de données : Utilisation de l'API yfinance pour récupérer les cours de clôture ajustés (Adj Close), intégrant ainsi les dividendes et les splits d'actions pour une précision financière optimale.

Architecture modulaire : Création de fonctions réutilisables pour le téléchargement, le calcul du Beta via des matrices de covariance (numpy.cov), et la génération de tableaux de bord financiers (pandas.DataFrame).

Visualisation : Normalisation des données en Base 100 pour comparer visuellement les trajectoires de performance de titres aux prix nominaux hétérogènes.

3. Indicateurs calculés

Volatilité : Mesure de l'incertitude via l'écart-type des rentabilités journalières.

Beta (β) : Mesure de la sensibilité du portefeuille par rapport aux mouvements du CAC 40.

Alpha (α) : Mesure de la valeur ajoutée réelle de la sélection d'actifs (stock picking).

4. Conclusion de l'étude L'analyse a mis en évidence des limites méthodologiques importantes, notamment la difficulté de comparer des titres technologiques américains (Nasdaq) au marché français sans neutraliser l'effet de change, celui-ci ayant agi comme une couverture naturelle sur la période étudiée.
