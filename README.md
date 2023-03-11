# Probabilité en pyhton
les cours de math, c'est bien mais comprendre c'est mieux!
vous pourrez trouver le code permettant de verifier la loi binomiale et sa convergance vers la loi normale pour n grand 

## Principe
on realise n tirages avec une probabilité de succes p
on compte le nombre de succes. C'est notre statistique X.
L'image ci-dessous represente les succes et les echecs 20 epreuves repetées 10 fois

```
n = 20
nb_tirages = 10
p=0.3

```

![](https://github.com/LouisDelprat/probabilit-en-python/blob/main/exemple_tirage.PNG)

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

![](https://github.com/LouisDelprat/probabilit-en-python/blob/main/proba_exemple1.PNG)


### n petit, beaucoup de tirages.
```
n = 5
nb_tirages = 100000
p=0.3
 ```
on voit que la loi binomiale( courbe vert) permet de predire la valeur mesurée par les tirages (barres bleues).
Par contre la loi normale (courbe violette) ne fonctionne dans cet exemple car n est trop petit

![](https://github.com/LouisDelprat/probabilit-en-python/blob/main/proba_exemple2.PNG)





### n grand, peu de tirages.
```
n = 50
nb_tirages = 10
p=0.3
 ```
on voit que la loi binomiale( courbe vert) et la loi normale( courbe violette) sont identiques car n est grand.
Par contre on n'a pas fait assez de tirages(nb_tirages petit) donc les probabilités mesurées n'ont pas cpnverges vers la loi binomiale. 
![](https://github.com/LouisDelprat/probabilit-en-python/blob/main/proba_exemple3.PNG)



# Conclusion

Ce programme nous permet de mieux comprendre et de visualiser les lois de probabilité.
Pour des tirages binaires ( succes/ echecs) les experiences convergent toujours vers la loi binomiale mais on ne peut le voir que si on repete l'experience beaucoup de fois (nb_tirages grand).
Quand n est grand la loi binomiale converge vers la loi normale.
