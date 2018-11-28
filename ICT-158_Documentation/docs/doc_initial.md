# Documentation initial

## Adressage ip
|Nom|Adresse|Masque de sous-réseau|
|---|-------|---------------------|
|ICT158-SRV03-1|10.1.1.20|255.255.255.0|
|ICT158-CLI7-1|via DHCP||

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

|Nom|Nom d'ouverture de session|Groupes|Chemin du profil|Chemin personnel|Script d'ouverture de session|
|---|--------------------------|-------|----------------|----------------|--------------------------------------|
|Mélanie Alonso|Melanie.alonso|Utilisateurs du domaine|\\\\ICT158-SRV03-1\Profils$\Melanie.alanso|\\\\ICT158-SRV03-1\Utilisateurs$\Melanie.alonso|Script_Back.vbs|
|Dana Schipper|Dana.Schipper|Utilisateurs du domaine|\\\\ICT158-SRV03-1\Profils$\Dana.Schipper|\\\\ICT158-SRV03-1\Utilisateurs$\Dana.Schipper|Script_Compta.vbs|
|Marc Mueller|Marc.Mueller|Utilisateurs du domaine|\\\\ICT158-SRV03-1\Profils$\Marc.Mueller|\\\\ICT158-SRV03-1\Utilisateurs$\Marc.Mueller|Script_Direction.vbs|
|Tim Brown|Tim.Brown|Utilisateurs du domaine<br>  IT|\\\\ICT158-SRV03-1\Profils$\Tim.Brown|\\\\ICT158-SRV03-1\Utilisateurs$\Tim.Brown|Script_IT.vbs|
|Jean-Michel Blaser|Jean-Michel.Blaser|Utilisateurs du domaine<br> Logistique|\\\\ICT158-SRV03-1\Profils$\Jean-Michel.Blaser|\\\\ICT158-SRV03-1\Utilisateurs$\Jean-Michel.Blaser|Script_Logistique.vbs|
|André Dupré|andre.dupre|Utilisateurs du domaine|\\\\ICT158-SRV03-1\Profils$\andre.dupre|\\\\ICT158-SRV03-1\Utilisateurs$\andre.dupre|Script_Marketing.vbs|
|Juerg Haefeli|Juerg.haefeli|Utilisateurs du domaine|\\\\ICT158-SRV03-1\Profils$\Juerg.haefeli|\\\\ICT158-SRV03-1\Utilisateurs$\Juerg.haefeli|Script_Production.vbs|
|Admin|Admin|Utilisateur|-|-|-|

### DNS
#### Zones de recherche directes

* \_msdcs.Scuolapro.local
* Scuolapro.local

#### Zones de recherche inversée
Pas de zone de recherche inverse configurée.
### DHCP

Étendue 10.1.1.0 :
  * Pool d'adresse :
    * Début : 10.1.1.40
    * Fin : 10.1.1.199
  * Option d'étendue :
    * Routeur : 10.1.1.1
    * Serveure DNS : 10.1.1.20
    * Nom de domaine DNS : ScuolaPro.local

### Scripts
|Non|Description|
|---|-----------|
|Script_Back.vbs|Attribue à la personen du back-office une imprimante et le partage qui lui est dédié|
|Script_Compta.vbs|Attribue à la personen de la comptabilité une imprimante et le partage qui lui est dédié|
|Script_Direction.vbs|Attribue à la personen de la direction une imprimante et le partage qui lui est dédié|
|Script_IT.vbs|Attribue à la personen de l'IT une imprimante et le partage qui lui est dédié|
|Script_Logistique.vbs|Attribue à la personen de la logictique une imprimante et le partage qui lui est dédié|
|Script_Merketing.vbs|Attribue à la personen du marketing une imprimante et le partage qui lui est dédié|
|Script_Production.vbs|Attribue à la personen de la production une imprimante et le partage qui lui est dédié|



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

##### ICT158-CLI7-1
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

##### ICT158-SRV03-01

|Nom|Éditeur|Version|
|---|-------|-------|
|Windows Server 2003 Services Pack 2|Microsoft Corporation|20070217.021435|
|Microsoft Visual C++ 2008 Redistributable - x86|Microsoft Corporation|9.0.30729.4148|
