# 4BDAV

## Exercice 1 day 1 :


### 3.Y a-t-il un ordre à respecter lors de la création de ces tables, si oui lequel ? Pourquoi ?
Oui, il faut tout d'abord créer les clés primaires auxquelles les tables vont faire référence, puis créer les clés étrangères dans l'ordre qui nous arrange pour ne pas faire appel a une colonne qui n'existe pas encore par exemple.

### 4. vérifier la structure grace à desc [nomDeTable]

![image](https://user-images.githubusercontent.com/47149398/171142659-d65710bc-c313-4915-9b3d-27abecc82c60.png)


### 5.Vider toutes vos tables. Y a-t-il un ordre à respecter ? Si oui, pourquoi ?
A moins de mettre un système de structure de données "on cascade", essayer de supprimer une valeur qui est référencée quelque part nous empechera d'executer la commande en nous indiquant qu'il existe encore une référence.
Ordre de suppression conseillé : 
(commencer par les tables qui ont des clés étrangères, finir avec celles qui ont uniquement des clés primaires : 
- det,
- pro, 
- com,
- fou,
- cli.
