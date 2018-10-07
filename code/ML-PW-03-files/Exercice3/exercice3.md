# Exercice 3
**auteurs : Costa Pedro, Delabays Louis, Guerne Jonathan**

## Exercice 3.1 
**Solution pour un classifieur d'image avec Bayes**

Les probabilités a priori (prior) vont se calculer de la même manière que pour l'exercie 1 de ce TP i.e. on va regarder la répartition des classes dans l'ensemble d'entraînement. 

La procédure se complexifie maintenant légèrement quand il s'agit de calculer la varaisemblance. Il serait trop couteux d'utiliser chaqu'un des pixels de l'image comme une feature et de générer ensuite un histogramme par feature. On va donc ajouter une étape de prétraitement qui va consister à extraire des features de chaqu'une des images. 

Comme il y aura moins de features on pourra cette fois utiliser des histogrammes pour définir la probabilité d'appartenance d'une valeur à une classe. Nous utiliserons ensuite la même hypothèse naïve d'indépendence des features pour pouvoir obtenir un résultat tenant compte de plusieurs features (voir exercie 1).