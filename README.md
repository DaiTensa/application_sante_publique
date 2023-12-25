# Projet 03 : Open Food Facts application au service de la santé publique

<span style="font-size:16px;">Notre jeu de données est composé de **`320772 lignes`**, qui correspondent au **`nombre de produits enregistrés`**, et **`162 colonnes`** qui décrivent les différentes **caractéristiques et composition de chaque produit**. </span>

<span style="font-size:16px;">Nous remarquons que **plusieurs features sont complètement vides :  0 not-null**, nous regarderons plus tard en détail ces colonnes pour décider si nous devons les garder ou supprimer. 
    
<span style="font-size:16px;">Il existes des **erreurs de "Typage"**, exemple ( **Les dates** ne sont pas au bon format **object -> datetime** ), (la variable **"quantity"** : **object -> intger ou classes** ), (**serving_size : object -> float ou int**), (**ingredients_from_palm_oil_tags : object -> float ou int**), 
(**ingredients_that_may_be_from_palm_oil_tags : object -> float**), (**nutrition_grade_fr : object -> float ou int**).</span> 

<span style="font-size:16px;">Des données manquantes de la variable **code** du produit, en effet, dans notre data frame nous disposons que **320749 codes produits**, contre **320772 enregistrements**, il s'agit surêment de données non rensegnées, nous les supprimerons dans ce cas.</span> 

<span style="font-size:16px;">Les autres variables semblent être au bon format.</span> 