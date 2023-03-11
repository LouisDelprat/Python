# Probabilité en pyhton
les cours de math, c'est bien mais comprendre c'est mieux!
vous pourrez trouver le code permettant de verifier la loi binomiale et sa convergance vers la loi normale pour n grand 

## Principe
on realise n tirages avec une probabilité de succes p
on compte le nombre de succes. C'est notre statistique X.
La loi binomiale permet de calculer la probabilité d'avoir k succes 
elle est noté X ~B(n,k)

## Resulats
### n grand, beaucoup de tirages
```
n = 50
nb_tirages = 100000
p=0.3
 ```

on voit que la loi binomiale(courbe vert) permet de predire la valeur mesurée par les tirages (barres bleues).
il n'y a pas de difference visble entre la loi binomiale et la loi normale (courbe violette) ne fonctionne dans cet exemple car n est trop petit











### n petit, beaucoup de tirage.
```
n = 5
nb_tirages = 100000
p=0.3
 ```
on voit que la loi binomiale( courbe vert) permet de predire la valeur mesurée par les tirages (barres bleues).
Par contre la loi normale (courbe violette) ne fonctionne dans cet exemple car n est trop petit

![](https://github.com/LouisDelprat/probabilit-en-python/blob/main/proba_exemple1.PNG)
