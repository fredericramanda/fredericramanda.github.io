+++
fragment = "content"
weight = 100

title = "Installation"

[sidebar]
  sticky = true
+++

## Spécifications techniques

Les spécifications suivantes évoluent selon la dimension de l'entreprise/organisation.

### Matériels

Des ordinateurs modernes avec architecture 64 bits.
Mémoire RAM : 4 Go au minimum.
Disque Dur : +50Go de libres.

* Si mono-poste

  * Un PC avec les spécifications ci-dessus
  * Une imprimante rattachée ou accessible à ce PC pour l'impression des documents

* Si PC en réseau

  * Un PC servant de serveur de base de données: sous Windows ou Linux
  * Des PC de travail sous Windows (Windows 7 au minimum)

### Système d’exploitation

YZYHRM fonctionne sur Window 7/10 ou Windows Server 2016, version 64 bits.
Le serveur de base de données: sous Windows ou Linux

## Logiciels préalables

### Le Serveur de Base de données HFSQL/Server

Utile si version Entreprise ou plus.

### Excel

Le logiciel Microsoft Excel est utile pour les imports/Exports.
Nous pourrons adapter YZYHRM pour Libreoffice plus tard et selon vos besoins.

### Installation du serveur

#### HFSQLDB

Nous nous chargerons de cette installation.

#### L'installateur de référence

Pour la version entreprise, une installation de référence est faite sur le serveur, accessible en écriture en réseau, et/ou partagé via Samba si Linux.


A chaque livraison d'une nouvelle version, cette version de référence sera mise à jour.

Après cela, dès qu'un utilisateur lance le logiciel, sa version est mise à jour automatiquement.

Cette installation de référence se charge aussi de toute modification de la structure de la base de donénes

#### Préparation de la base de données

* Pour la version standard

Une base de données modèle est déjà fournie. Les utilisateurs n'auront qu'à vérifier les paramètres et commencer à travailler.

* Pour la version Entreprise

Nous nous chargerons d'auditer votre système de paie et créerons et paramétrons votre base de données.

Si multi-bases, nous vous fournirons des outils pour leur création.

Une base de données des utilisateurs et droits est installée au niveau du serveur.

#### Installation du logiciel

**Installation du logiciel**


* Aller sur le dossier de partage contenant l'installateur de référernce.

* Lancer l'exécutabel **install.exe**.

* Copier le fichier apps.ini, permettant de pointeger vers la base des droits/utilisateurs

* Lancer l'application ensuite

**Mise à jour du logiciel**

Se fait automatiquement dès que l'installation de référence est mise à jour.

Aucune action de la part de l'utilisateur.


### Configurer le logiciel


Pour la version standard, l'utilisateur aura à configurer la société

Pour la version Entreprise nous nous chargerons de toute la configuration:

* société et identité
* paramétrage de la paie
* importation des agents actifs
* paramétrage et configurations diverses (schéma comptable...)

***Remarque***

Ce manuel est en cours de finalisation.