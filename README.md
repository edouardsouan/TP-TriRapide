# TP-TriRapide

###Questions V3 : 
2) 	Le fait de retourner la somme des tâhes oblige les pools à'attendre et reproduit l'effet d'un join sur un Thread classique.

Le problèe de synchronisation de la question 1 est donc réolu. 

 4) La V3 est extrêment plus efficace que la V2 pour les grands volumes de données (1million). La V3 n'a mis qu'une minute trente pour trier le tableau alors que la V2 n'a pas réussi en plus de 15 min. 
Ce n'est pas réellement étonnant dans la mesure ou la V3 économise la création de nombreux threads. 

5) La V1 est plus efficace que la V2 et la V3 pour un petit volume de données ( 10000). La V2 et la V3 ne change pas vraiment au niveau performance jusqu'a environ 100000 données et passé la barre du million, la V3 est largement plus efficace que la V1 et V2. 

Une solution serait de tester la longueur du tableau de donnés et lorsque celle-ci atteint une taille de l'ordre du millier de données, utiliser la V1 et pour le reste utiliser la V3. 