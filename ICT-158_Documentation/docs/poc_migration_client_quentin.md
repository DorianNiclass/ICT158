#POC Migration client

## Création d'une image windows 10

## Mise en place des services de déployement d'os et d'application
* Ajout du rôle **Serveur d'applications**
* Ajout du rôle **Services de déploiement Windows**

## Configuration du service de déployement

* Option d'installation : Intégré à l'Active Directory
* Dossier d'installation distant : **C:\RemoteInstall**
* Paramètres initiaux du serveur PXE : Répondre à tous les ordinateurs clients (Connus et inconnus) et Exiger l'approbation administrateur pour les ordinateurs inconnus.
