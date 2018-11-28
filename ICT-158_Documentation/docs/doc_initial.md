# Documentation initial

## Adressage ip
|Nom|Adresse|Masque de sous-réseau|
|---|-------|---------------------|
|ICT158-SRV03-1|10.1.1.20|255.255.255.0|
## Configuration ICT158-SRV03-1


### Configuration
* Marque : HP Proliant DL380 Gen5
* Nom : ICT158-SRV03-1
* Système d'exploitation : Windows server 2003
* CPU : Intel Core I7 6700 3.4 Ghz
* Nombre de coeur : 1
* RAM : 512 Mo
* Disques durs :
  * Disque 1 : 40Go
  * Disque 2 : 40Go
  * Disque 3 : 40Go
  * Disque 4 : 40Go

### Configuration réseau
* Ip : 10.1.1.20
* Masque de sous-réseau : 255.255.255.0
* Serveur DNS : 10.1.1.20
* Passerelle par défaut : 10.1.1.1
* Domaine : Sculapro.local

### Services installés
* Serveur de fichier
* Serveur d'impression
* Active directory
* DNS
* DHCP


### Serveur de fichier
#### Partages
|Nom|Chemin|Caché|
|---|------|:---:|
|ADMIN$|C:\WINDOWS|✓|
|C$|C:\ |✓|
|D$|D:\ |✓|
|Downloads|D:\Downloads||
|Echange|D:\Echange||
|IPC$||✓|
|NETLOGON|C:\WINDOWS\SYSVOL\sysvol\Scuolapro.local\SCRIPTS||
|print$|C:\WINDOWS\system32\spool\drivers|✓|
|Profils$|D:\Profils|✓|
|Services|D:\Services||
|SYSVOL|C:\WINDOWS\SYSVOL\sysvol||
|Utilisateurs$|D:\Utilisateurs|✓|


### Serveur d'impression

Liste des imprimantes

|Nom|Adresse IP|
|---|----------|
|HP_Back|10.1.1.206|
|HP_Compta|10.1.1.201|
|HP_Direction|10.1.1.204|
|HP_IT|10.1.1.200|
|HP_Log|10.1.1.202|
|HP_Marketing|10.1.1.205|
|HP_Prod|10.1.1.203|

### Active directory

#### Configuration AD

* Nom de domaine : Scuolapro.local
* Nom de domaine (antérieur à Windows 2000) : SCUOLAPRO
* Niveau fonctionnel du domaine : Windows 2000 mixte
* Niveau fonctionnel de la forêt : Windows 2000

#### Groupes AD

|Nom|
|---|
|Accès compatible pré-Windows 2000|
|Administrateurs|
|Duplicateurs|
|Générateurs d'approbations de forêt entrante|
|Groupe d'accès d'autorisation Windows|
|Invités|
|Opérateurs d'impression|
|Opérateurs de compte|
|Opérateurs de configuration réseau|
|Opérateurs de sauvegardes|
|OPérateurs de serveur|
|Serveurs de licenses des services Terminal Server|
|Utilisateurs|
|Utilisateurs de l'Analyseur de performances|
|Utilisateurs du Bureau à distance|
|Utilisateurs du journal de performances|
|Utilisateurs du modèle COM distribué|
|Back-Office|
|Comptabilite|
|Direction|
|IT|
|Logistique|
|Marketing|
|Production|

#### Utilisateurs AD

|Nom|Nom d'ouverture de session|Groupes|
|---|--------------------------|-------|
|Mélanie Alonso|Melanie.alonso|Utilisateurs du domaine|
|Dana Schipper|Dana.Schipper|Utilisateurs du domaine|
|Marc Mueller|Marc.Mueller|Utilisateurs du domaine|
|Tim Brown|Tim.Brown|Utilisateurs du domaine<br>  IT|
|Jean-Michel Blaser|Jean-Michel.Blaser|Utilisateurs du domaine<br> Logistique|
|André Dupré|andre.dupre|Utilisateurs du domaine|
|Juerg Haefeli|Juerg.haefeli|Utilisateurs du domaine|
|Admin|Admin|Utilisateur|

### DNS
#### Zone de recherche directes

\_msdcs.Scualopro.local :

### DHCP

Étendue 10.1.1.0 :
  * Pool d'adresse :
    * Début : 10.1.1.40
    * Fin : 10.1.1.199
  * Option d'étendue :
    * Routeur : 10.1.1.1
    * Serveure DNS : 10.1.1.20
    * Nom de domaine DNS : SculaPro.local



## Configuration ICT158-CLI7-1

* Marque : Dell Latitude E6510
* Nom : ICT158-CLI7-1
* Système d'exploitation : Windows 7 Entreprise
* CPU : Intel Core I7 6700 3.4 Ghz
* Nombre de coeur : 1
* RAM : 2048 Mo
* Disques durs :
  * Disque 1 : 60Go

### Logiciels

|Nom|Éditeur|Version|
|---|-------|-------|
|Bonjour|Apple Inc.|2.0.4.0|
|Adobe Acrobat Reader DC - Français|Adobe Systems Incorporated|15.017.20050|
|Gadwin PrintScreen (64-Bit)|Gadwin Systems|5.4.2.0|
|Avira Launcher|Avira Operations GmbH & Co. KG|1.2.71.21096|
|XMind 7.5 Update 1|XMind Ltd.|3.6.51.201607142338|
|Mozillia Maintenance Service|Mozilla|49.0.1|
|Mozillia Firefox|Mozilla|49.0.1|
|Avira Antivirus|Avira Operations GmbH & Co. KG|15.0.20.59|
|PDFCreator|pdfforge GmbH|2.3.2|
|UltraVnc|uvnc bvba|1.2.1.1|
|Module linguistique Microsoft .NET Framework 4 Client Profile Français|Microsoft Corporation|4.0.30319|
|Microsoft .NET Framwork 4 Client Profile|Microsoft Corporation|4.0.30319|
|Microsoft Office Professional Edition 2003|Microsoft Corporation|11.0.5614.0|
|Microsoft Visual C++ 2008 Redistributable - x64|Microsoft Corporation|9.0.30729.6161|
|Microsoft Visual C++ 2008 Redistributable - x86|Microsoft Corporation|9.0.30729.4148|
