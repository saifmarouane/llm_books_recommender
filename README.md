
# Système de Recommandation de Livres Basé sur le Filtrage de Contenu et les Embeddings BERT

## Description du Projet
Ce projet implémente un système de recommandation de livres basé sur le filtrage de contenu. Il utilise une combinaison de techniques telles que **TF-IDF**, **KeyBERT** et **BERT embeddings** pour améliorer la qualité des recommandations, et **GPT** pour une interaction conversationnelle avec les utilisateurs.

### Fonctionnalités Principales :
- **Extraction de caractéristiques textuelles** : En utilisant TF-IDF pour extraire la fréquence et la pertinence des termes dans les descriptions des livres.
- **Extraction de mots-clés** : Utilisation de KeyBERT pour extraire des mots-clés pertinents à partir des embeddings BERT.
- **Calcul de la Similarité Cosinus** : Pour comparer les livres en utilisant des vecteurs numériques et générer des recommandations.
- **Interaction avec GPT** : Ajout de GPT pour offrir des recommandations personnalisées via une interface conversationnelle.

## Structure du Projet

### 1. Extraction et Représentation des Caractéristiques Textuelles
#### 1.1 Approches de Traitement des Données
- **TF-IDF** : Utilisé pour mesurer l'importance des termes dans les descriptions des livres. La fréquence d’un terme (TF) dans un document est multipliée par son importance globale dans le corpus (IDF).
  
- **KeyBERT** : Algorithme d'extraction de mots-clés basé sur les embeddings BERT. Il génère des embeddings pour les descriptions des livres et sélectionne les termes les plus pertinents.

#### 1.2 Avantages de l’Utilisation de KeyBERT avec TF-IDF
- **Représentation Sémantique Améliorée** : KeyBERT permet de capturer la sémantique des termes, améliorant ainsi la précision de l'extraction des mots-clés.
- **Flexibilité** : KeyBERT permet l'ajustement des embeddings pour s'adapter aux besoins spécifiques du corpus de livres.

### 2. Construction de la Matrice de Similarité et Génération de Recommandations
#### 2.1 Calcul de la Similarité Cosinus
Une **matrice de similarité cosinus** est construite pour comparer les vecteurs numériques représentant chaque livre et identifier ceux qui sont les plus similaires.

#### 2.2 Génération de Recommandations
Les recommandations sont générées en fonction de la similarité des descriptions de livres, en tenant compte des mots-clés extraits et des vecteurs numériques.

### 3. Intégration de GPT
Le modèle GPT est utilisé pour permettre une interaction conversationnelle avec les utilisateurs, en générant des recommandations plus personnalisées et en s’adaptant aux préférences exprimées en temps réel.

## Utilisation du Projet
1. **Extraction des mots-clés** : Utilisez les méthodes TF-IDF et KeyBERT pour extraire les mots-clés des descriptions des livres.
2. **Calcul de la Similarité** : Construisez des vecteurs pour chaque livre et calculez la similarité cosinus pour identifier les livres similaires.
3. **Recommandation** : Utilisez la matrice de similarité pour générer des recommandations de livres.
4. **Interaction avec GPT** : Intégrez GPT pour une interaction conversationnelle, permettant à l'utilisateur de recevoir des recommandations plus personnalisées.

## Technologies Utilisées
- **Python** : Langage de programmation principal.
- **BERT** : Modèle de langage pour générer des embeddings.
- **KeyBERT** : Pour extraire les mots-clés basés sur les embeddings BERT.
- **TF-IDF** : Pour mesurer la fréquence et la pertinence des termes.
- **GPT** : Modèle de génération de texte pour améliorer l'interaction utilisateur.

## Auteurs
Ce projet a été développé pour démontrer l'efficacité du filtrage de contenu et des modèles de langage avancés pour la recommandation de livres.
