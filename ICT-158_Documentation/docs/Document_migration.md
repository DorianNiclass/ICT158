
# Document de planification de la migration - ScuolaPro

## Introduction

Planification de la migration du Windows Server 2003 vers un Windows Server 2012 R2.
Le matériel, les données et les services devront, dans la mesure du possible, être migrés sans interruption de service.

## Migration des données

3 méthodes

### Méthode 1 - Via supports externes

Utiliser un média externe (clé USB, disque dur externe, etc...) sur lequel on copie les données du Windows Server 2003 afin de pouvoir les transférer sur le Windows Server 2012 R2.

|Avantages|Inconvénients|
|---------|-------------|
| - Ne nécessite pas de mettre en place un quelconque système|- Transfère assez long suivant la taille des données <br> - Si les utilisateurs modifies certaines données durant le transfère, ces modification seront perdues |

### Méthode 2 - Transfère via le réseau

Transférer les données via le réseau en utilisant les partages. Cet opération peut être automatisée avec un script, qui sera exécuté durant la nuit lorsque plus personne ne sera amenée à utilisé ces données.

|Avantages|Inconvénients|
|---------|-------------|
|- Automatisé avec un script|- Limité par la vitesse du réseau|

### Méthode 3 - Déplacer les disques durs

Déplacer directement les disques durs contenant les données sur le Windows Server 2012 R2.

|Avantages|Inconvénients|
|---------|-------------|
|- Transfère rapide <br> - Pas besoin de racheter des disques durs|- Les données sont temporairement indisponible <br> - Nécessite une interuption des services|


## Migration des services

## Matériel
### Prérequis matériel Windows Server 2012 R2
Windows server 2012 R2 à besoin au minimum :
* CPU : 1.4 GHz 64-Bit
* RAM : 512 Mo
* Disque : 32 Go
* Carte réseau : 10/100/1000baseT

#### Note
Windows Server 2012 R2 aura besoin de plus de place sur le disque dur si il y a 16 Go de RAM ou plus installé pour les mémoires tempons, etc...
