+++
fragment = "content"
weight = 100

title = "Installation"

[sidebar]
  sticky = true
+++

## Spécifications techniques

Les spécifications suivantes supposent une installation au niveau d'une Commune de taille réduite.

### Matériels

Des ordinateurs modernes avec architecture 64 bits.
Si le service des Etats Civils disposent de plus d’un ordinateur, il faut que ceux-ci soient mis en réseau.
Il est préférable de mettre des « dongles wifi » sur chaque poste.
Mémoire RAM : 4 Go au minimum.
Disque Dur : +50Go de libres.

* Si mono-poste

  * Un PC avec les spécifications ci-dessus
  * Une imprimante rattachée ou accessible à ce PC pour l'impression des documents

* Si PC en réseau

### Système d’exploitation

Le logiciel Vitalis, dans sa version actuelle, fonctionne sur Window 10 ou Windows Server 2016, version 64 bits.

## Logiciels préalables

### Installations communes

Les installations suivantes sont communes à chaque poste, simple poste ou serveur (voir architecture).

* Microsoft Office
Il faut que chaque poste de travail dispose de Microsoft Office version 2007 au moins.
* Navigateurs : Firefox ou Chrome
Installer le navigateur Firefox ou Chrome sur chaque poste.

***Remarque:*** Dans une future version, nous préparerons des versions avec Linux et des logiciels comme LibreOffice.

### Installation du serveur

#### Serveur Email
Si la Commune n’a pas de serveur Email, il est nécessaire de tenir compte des impératifs suivants :
Il n’est pas possible de modifier les mots de passe des utilisateurs sans passer par un serveur Email qui va recevoir les données y afférente.

#### Postgresql

* Installer Postgresql :
Lancer le logiciel d’installation « postgresql-12.1-1-windows-x64.exe ».
![image alt text](/images/vitalis/pg_001.png)
</br>Faire « suivant »
</br>Choisir le répertoire d’installation : NE PAS CHANGER et faire suivant
![image alt text](/images/vitalis/pg_002.png)
</br>Cocher les éléments à installer : NE RIEN CHANGER et faire suivant
![image alt text](/images/vitalis/pg_003.png)
* ndiquer le mot de passe de l’utilisateur « postgres », confirmer répéter en bas. 
</br>***SE SOUVENIR de ce mot de passe.***
* Indiquer le port : NE PAS CHANGER (5432)
* Choisir la langue locale : NE PAS CHANGER
* Faire suivant et attendre que l’installation se termine.
* Ne rien faire quand il demande de lancer Stack Builder.

#### Préparation de la base de données

Lancer le logiciel pgAdmin 4.</br>
Normalement il va ouvrir le navigateur par défaut.</br>
</br>
</br>
![image alt text](/images/vitalis/pg_004.png)
Veuillez indiquer un mot de passe maitre : ***IL FAUT SE SOUVENIR DE CE MOT DE PASSE*** (le noter quelque part). Ce mot de passe est demandé à chaque démarrage de pgAdmin4</br>

Cliquer sur le nœud Servers</br>
Cliquer sur le nœud Login/Group Roles et choisir Create -> Login/group Role…</br></br>
![image alt text](/images/vitalis/pg_005.png)
Créer utilisateur : vitalis avec un mot de passe ***IL FAUT SE SOUVENIR DE CE MOT DE PASSE***</br>
![image alt text](/images/vitalis/pg_006.png)</br></br>
Aller dans l’onglet Définition, et saisir le mot de passe. Ne rien changer en bas.</br>
![image alt text](/images/vitalis/pg_007.png)</br></br>
Aller dans l’onglet Privileges et tout cocher pour avoir YES partout :</br>
![image alt text](/images/vitalis/pg_008.png)
</br>
</br>
**Créer base de données : vitalis**
</br>Aller dans le nœud « Databases »
</br>Clic droit et choisir Create -> Database…
</br>
</br>
![image alt text](/images/vitalis/pg_009.png)
</br>
</br>
</br>Indiquer le nom de la base de données : **vitalis**
</br>Choisir le « owner » (propriétaire) et mettre l’utilisateur créé tout à l’heure : **vitalis**
</br>Mettre un commentaire si nécessaire : **base de données pour le logiciel Vitalis**
</br>Cliquer sur le bouton : **Save**
</br>
</br>
![image alt text](/images/vitalis/pg_010.png)
</br>
</br>
**Importation de la structure initiale de la base :**
</br>Une structure initiale a été créée et  doit etre importée dans la base vitalis.
</br>Voir le fichier « vitalis_initial.backup » dans le dossier contenant livraisons/intial/data.
</br>Pour cela, chercher le nœud « vitalis » dans « Databases »,
</br>Faire un clic droit et choisir « Restore » :
</br>
</br>
![image alt text](/images/vitalis/pg_011.png)
</br>
</br>
1. Rechercher le fichier de backup tout à l’heure en cliquant sur le bouton de la ligne « Filename »
2. Rechercher l’utilisateur Vitalis pour le « role name ».
3. Et faire « restore »
</br>Laisser le processus se terminer normalement.
</br>
</br>
**Vérification de la base de données**
</br>
</br>
Il faut cliquer sur le nœud Databases, vitalis, Tables et vous devez voir les tables de données, comme indiquées :
</br>
</br>
![image alt text](/images/vitalis/pg_012.png)

#### Installation du logiciel

**Préparation des dossiers**


Pour mieux gérer le logiciel, préparer un dossier dans la racine d’un lecteur du disque dur.
</br>Ex : Lecteur **D:\**
</br>Dossier racine : **d:\vitalis** ou **d:\vitalis**

**Installation du logiciel**

</br>Le logiciel vient comme un fichier compressé au format zip ou 7zip.
</br>Selon les cas :
</br>• La version complète
arsf_new.zip ou vitalis_new.zip
</br>• Ou une version de mise à jour
</br>arsf_update.zip ou vitalis_update.zip
</br>Ouvrir ce fichier via 7zip Tools ou Winrar ou l’outil intégré de Windows et décompresser vers le dossier racine préparé ci-dessus.
</br>Normalement, on doit obtenir la structure suivante :


![image alt text](/images/vitalis/install_001.png)


Le fichier vitalis.cmd permet de lancer le logiciel.
</br>Le sous-dossier bin contient le logiciel, un fichier de configuration local.env et un dossier des logs (traces d’exécution du logiciel).

![image alt text](/images/vitalis/install_002.png)


1. Le logiciel

Vitalis vient comme un fichier compressé au format zip (ou 7zip).</br>
Pour cela il faut disposer d'un logiciel de décompression ou se servir de l'outil de décompression integré dans Windows.



### Configurer le logiciel



Entre autres configurations, il faut ouvrir avec un éditeur de texte, comme notepad, le fichier local.env :


![image alt text](/images/vitalis/install_003.png)


Se placer sur la ligne **DATABASE_URL=postgres**, et modifier les mots suivants :
</br>user : le nom de l’utilisateur de la base de données (voir paragraphe postgresql, normalement vitalis)
</br>motdepasse : le mot de passe de l’utilisateur
</br>database : le nom de la base de données (voir paragraphe postgresql, normalement vitalis)
</br>Enregistrer les modifications et fermer le fichier


### Lancer le logiciel

Se placer dans le dossier contenant le fichier vitalis.cmd
* Ouvrir le logiciel Invite de Commande
* Changer de lecteur en tapant **d:\**
* Entrer dans le dossier **cd vitalis**
* Lancer le logiciel en tapant **vitalis.cmd**.

![image alt text](/images/vitalis/install_004.png)


Si tout se passe bien, le logiciel peut être lancé sur le poste serveur dans le navigateur en tapant l’adresse url suivant :
</br>http://localhost:8000.
</br>Pour lancer sur un autre poste, voir le manuel d’utilisation.


## Paramétrer le logiciel


### Contenu initial


Utilisateurs :

* admin@macommune.mg (mot de passe admin2019)</br>
* user@macommune.mg (mot de passe user2019)


Dès le premier login, il faut modifier ces mots de passe.

### Autres configurations

* Modèles de document : tous les modèles requis utilisés par le logiciel.
* Vérifier les configurations : Il faut mettre le ou les officiers de l’Etat Civil

### Divers

Il faut procéder à la sauvegarde des bases de données et fichiers du serveur régulièrement (hebdomadaire et journalière).
Pour cela, il faut apprendre à manipuler le logiciel ***pgAdmin*** qui permet de faire la sauvegarde.