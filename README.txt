README
- Auteur du projet : - Abdarare HÉRARD
- Date : 10 janvier 2026

STRUCTURE DU PROJET :
- ┌── Data
-       ├── customers.csv                                                  (données clients)
-       ├── products.csv                                                   (catalogue produits)
-       ├── order_lines.csv                                                (lignes de commande)
- ├── Scripts
-       ├── Chargement, Comprehension et nettoyage des donnees.ipynb       (inspection, nettoyage et préparation des données)
-       ├── ICP (Indicateur Clé de Performance).ipynb                      (calcul des indicateurs)
-       ├── Jointures (Merge) pour enrichir les ventes.ipynb               (enrichissement et analyse)
-       └── Main.ipnyb                                                     (centre de controle)
- ├── Livrables
-       ├── Données_nettoyées
-               ├── order_lines_clean.csv                                  (lignes de commandes nettoyées)
-               ├── products_clean_csv                                     (catalogue produits nettoyés)
-               └── customers_clean.csv                                    (données clients nettoyées)
-       ├── KPI_calculés
-               └── kpi_ca_mensuel.csv                                     (chiffres d'affaires mensuels)
-       └── Jointure_et_pivot table
-               ├── orders_enriched.csv                                    (données jointes et colonnes calculées ajoutées)
-               └── pivot_segent_category.csv                              (tableau pivot des chiffres d'affaires par segment et catégorie)
- ├── README.md
- └── Rapport.pdf  

ORDRE D'EXÉCUTION :
    - 1. Étape 1 et 2 : Comprendre les données brutes, identifier les problèmes et nettoyer les données (types, NaN, anomalies)
    - 2. Étape 3 : Calculer les KPI (CA, panier moyen, taux de retour, etc.)
    - 3. Étape 4 : Enrichir avec jointures et analyser par segment/catégorie
   
FICHIERS GÉNÉRÉS :
   • order_lines_clean.csv : données nettoyées
   • products_clean.csv 
   • customers_clean.csv 
   • kpi_ca_mensuel.csv : tableaux de bord des indicateurs
   • orders_enriched.csv : table finale enrichie
   • pivot_segment_category.csv : analyses croisées
   
### CONCEPTS PANDAS UTILISÉS :
   ✓ read_csv, head, info, describe, value_counts
   ✓ to_datetime, to_numeric, astype
   ✓ isna, fillna, dropna, duplicated, drop_duplicates
   ✓ groupby, agg, pivot_table, merge
   ✓ sort_values, nlargest, to_csv
   
### CONSEILS :
   - Exécuter les étapes dans l'ordre
   - Utiliser l'option 4 pour un traitement complet
