# Projet 03 : Open Food Facts application au service de la santé publique

L'agence ["Santé publique France"](https://www.santepubliquefrance.fr/) a lancé un appel à projets pour trouver des idées innovantes d’applications en lien avec l'alimentation. Vous souhaitez y participer et proposer une idée d’application.

<span style="font-size:16px;">Notre jeu de données est composé de **`320772 lignes`**, qui correspondent au **`nombre de produits enregistrés`**, et **`162 colonnes`** qui décrivent les différentes **caractéristiques et composition de chaque produit**. </span>

<span style="font-size:16px;">Nous remarquons que **plusieurs features sont complètement vides :  0 not-null**, nous regarderons plus tard en détail ces colonnes pour décider si nous devons les garder ou supprimer. 
    
<span style="font-size:16px;">Il existes des **erreurs de "Typage"**, exemple ( **Les dates** ne sont pas au bon format **object -> datetime** ), (la variable **"quantity"** : **object -> intger ou classes** ), (**serving_size : object -> float ou int**), (**ingredients_from_palm_oil_tags : object -> float ou int**), 
(**ingredients_that_may_be_from_palm_oil_tags : object -> float**), (**nutrition_grade_fr : object -> float ou int**).</span> 

<span style="font-size:16px;">Des données manquantes de la variable **code** du produit, en effet, dans notre data frame nous disposons que **320749 codes produits**, contre **320772 enregistrements**, il s'agit surêment de données non rensegnées, nous les supprimerons dans ce cas.</span> 

<span style="font-size:16px;">Les autres variables semblent être au bon format.</span> 

# Les données

Le jeu de données Open Food Facts est disponible sur [le site officiel](https://world.openfoodfacts.org/),
disponible en téléchargement à [ce lien](https://s3-eu-west-1.amazonaws.com/static.oc-static.com/prod/courses/files/parcours-data-scientist/P2/fr.openfoodfacts.org.products.csv.zip), les varaibles sont définies à [cette adresse](https://world.openfoodfacts.org/data/data-fields.txt)

Les champs sont séparés en quatre sections:
 - Les informations générales sur la fiche du produit : nom, date de modification, etc.
 - Un ensemble de tags : catégorie du produit, localisation, origine, etc.
 - Les ingrédients composant les produits et leurs additifs éventuels.
 - Des informations nutritionnelles : quantité en grammes d’un nutriment pour 100 grammes du produit.

# Compétences
 - Communiquer les résultats à l’aide de représentations graphiques lisibles et pertinentes.
 - Effectuer des opérations de nettoyage sur des données structurées.
 - Effectuer une analyse statistique multivariée.
 - Effectuer une analyse statistique univariée.