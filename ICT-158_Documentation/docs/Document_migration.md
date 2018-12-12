# Document de planification de la migration - ScuolaPro

## Introduction

Planification de la migration du Windows Server 2003 vers un Windows Server 2012 R2.
Le matériel, les données et les services devront, dans la mesure du possible, être migrés sans interruption de service.

## Migration des données

Nous proposons 3 méthodes différentes pour la migration des données.

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

Nous proposons 2 méthodes différentes pour la migration des services.

### Méthode 1 - Replications

Répliquer les services (DNS, DHCP, AD) et dupliquer les partages sur le nouveau serveur. Il faut pour cela mettre en place le nouveau serveur, le promouvoir en contrôleur de domaine, pratiquer la replication, dépromouvoir l'ancien serveur.
Le nouveau serveur reprendra l'entière responsabilité des services. Cette méthode permet une migration sans interuption de service.

|Avantages|Inconvénients|
|---------|-------------|
|- Pas d'interruption de service| - Long à mettre en place (il faut paramétrer les réplications sur tous les services et vérifier leur fonctionnement)|

### Méthode 2 - Copie des données des services

Copier et déplacer les bases de données AD, DNS et DHCP vers le nouveau serveur et les importer dans les nouveaux services. Il faut pour cela mettre en place le nouveau serveur et y installer les services. Pour pouvoir copier correctement les bases de données il faut stopper les services, ce qui ne garanti par une migration sans interruption de service.

|Avantages|Inconvénients|
|---------|-------------|
|- Plus rapide à mettre en place| - Ne garanti pas une migration sans interruption de service|
