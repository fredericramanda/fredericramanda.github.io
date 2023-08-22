+++
fragment = "content"
weight = 100

title = "Manuel d'utilisation"

[sidebar]
  sticky = true
+++

Le logiciel de gestion de l’Etat Civil Vitalis a été conçu est développé pour accompagner les Mairies et Communes
de Madagascar dans la gestion efficace du Registre de l’Etat Civil.
.

### Généralités

#### Législation et principes de l’Etat Civil

Ce logiciel est conforme à la législation de la République de Madagascar, portant sur l’organisation et la gestion
de l’Etat Civil.
En outre, ce logiciel s’attache à accompagner chaque Mairie et les utilisateurs pour :
* Assurer la saisie à temps des déclarations (naissance, décès...)
* Délivrer en temps record les copies, bulletins ou autres certificats demandés par les usagers.
* Conserver, rechercher et exploiter, dans la limite des réglementations existantes les données saisies sur
l’Etat Civil.

Il faut seulement remarquer que ce logiciel DOIT être utilisé en même temps avec les registres papiers
existants :
* Recherche simultanée dans les livres et le logiciel
* Annotation des mentions à la fois dans les livres et dans le logiciel.

Et enfin, Vitalis peut être adapté facilement pour d'autres pays.

#### Processus de gestion de l’Etat Civil

Ce logiciel est conforme au processus de gestion de l’Etat Civil communément pratiqué dans chaque Mairie du
Pays :
* Enregistrement à temps des déclarations
* Enregistrement selon leur arrivée des mentions, jugements rendus portant sur l’Etat Civil
* Délivrance de copies, bulletins ou certificats

En général les étapes se passent comme suit :
* Après un événement à déclarer (naissance, décès...)
* Arrivée du déclarant, des personnes concernée (mariés par exemple) et éventuellement d’autres
témoins avec les dossiers et pièces administratives utiles
* Enregistrement de l’acte
* Délivrance de la première copie
* Archivage d’une cope

Ou

* Arrivée d’un demandeur de copies/bulletins/certificats
* Recherche dans les livres et dans le logiciel
* Enregistrement de la demande
* Saisie initiale si nécessaire de l’acte (si non présent dans le logiciel) et avec les informations lues dans les
livres
* Délivrance de la/du copie/bulletin/certificat.


#### Acteurs, Responsables

* Officier de l’Etat Civil : responsable de la validation et signature des actes et copies
* Secrétaire de l’Etat Civil : responsable de la saisie, recherche, répondre aux demandes des usagers
* Usagers : responsable de la déclaration, origine des demandes, valident les contenus avant réception.
* Administrateur du logiciel : la Mairie doit désigner un administrateur du logiciel pour en assurer
paramétrage (utilisateurs, modèles...) et bon fonctionnement (installation, sauvegarde, restauration...)
* Editeur du Logiciel : responsable du développement, réalisation des correctifs et évolution du logiciel
* Partenaires : autres partenaires chargés de la réalisation et suivi du projet.

#### Fonctionnalites

Le logiciel Vitalis permet de gérer les types d’actes d’Etat Civil suivant :


* Naissance
  * Enregistrement des déclarations ou jugements supplétifs
  * Délivrance de copie, bulletin
  * Annotation et mentions
* Décès :
  * Enregistrement des déclarations
  * Délivrance de copie, bulletin
* Mariage
  * Enregistrement
  * Délivrance de copie, bulletin
* Séparation, divorce et annulation
  * Enregistrement du jugement
  * Délivrance de copie
* Divers : changements (naissance, nom), adoptions (reconnaissances, légitimation)
  * Enregistrement de la déclaration ou jugements
  * Délivrance de copie
* Certificats : délivrance de certificats LIES à l’Etat Civil
  * Certificat de filiation
  * ...

En outre, le logiciel permettra :

* La recherche d’actes et de tâches
* L’enregistrement de chaque tâche : une tâche est la matérialisation dans le logiciel d’une déclaration, ou
une demande de copie, de bulletins ou certificats
* Le reporting et statistique liés aux tâches et aux actes

### Ouvrir le logiciel

#### Ouverture initiale

Pour utiliser le logiciel, il faut nécessairement :
* Vérifier que le poste de travail contenant le logiciel soit allumé ou éventuellement le serveur
* Que votre poste soit connecté en réseau avec ce poste de travail (si ce n’est pas le même)
Après, il faut lancer le navigateur. Nous recommandons :
Firefox (version > 60) ou Chrome (>60) ou opera. Il ne faut pas utiliser d’autres navigateurs.


| ![firefox](/images/vitalis/manual_001_firefox.jpg)      |      ![chrome](/images/vitalis/manual_003_opera.png) |        ![chrome](/images/vitalis/manual_002_chrome.png)     |
|----------------------------|----------------------------|----------------------------|


Après ouverture du navigateur, tapez dans la barre d’adresse, l’adresse de l’application (son URL).
Cela pourrait être :

* ***http://127.0.0.1:8000*** : Si serveur sur le même poste
* ***http://nomserveur:8000*** : Il faut demander ce nom de serveur à l’administrateur
* ***http://XXX.XXX.XXX.XXX:8000/*** : Le n° IP du serveur ; il faut demander ce N° à l’administarteur

Le chiffre 8000 représente le port d’activation du serveur. Cela pourrait changer, et il faut le confirmer auprès de l’administrateur (exemples d’autres valeurs : RIEN, ou 8080…). RIEN veut dire port 80 et il faut enlever le deux-points devant.

#### Ecran de bienvenue

Après avoir tapez ENTRER dans la barre d’adresse, vous devez arriver à l’écran de bienvenue :

![Bienvenue](/images/vitalis/manual_004_bienvenue.png)

### Présentation du logiciel

#### L’écran principal

Après le login, l’utilisateur arrive normalement à cet écran :

![Bienvenue](/images/vitalis/manual_005_principal.png)

Dans cet écran vous avez les éléments principaux :
* Le logo personnalisable présentant le logiciel et ou la Commune
* Le nom de l’utilisateur avec un menu dessous si on y clique
* La page d’accueil (accessible via le menu Accueil)
* La barre de menu
* Une barre de recherche en haut (désactivé pour le moment)

#### La barre de menus à gauche

Cette barre peut s’afficher en entier (icons + textes) ou seulement avec les icons représentant chaque type d’actes et les autres fonctions principales du logiciel :

1. Ce bouton permet de cacher/afficher la barre de menu
2. La liste des menus. L’utilisateur se familiarisera rapidement avec chaque icon.

![Menu Gauche](/images/vitalis/manual_006_menu_gauche.png)

### Fonctionnalités communes

#### Menu Utilisateur

Dans le coin haut à droite, un menu apparait dès que l’utilisateur clique sur son nom :

![Menu User](/images/vitalis/manual_007_menu_user.png)

1. Permet de modifier les paramètres du logiciel (si administrateur)
2. Le profil de l’utilisateur : information sur l’utilisateur
3. Déconnecter permet de quitter l’application

**Profil**

Affiche les informations courtes sur l’utilisateur courant :

![Menu User](/images/vitalis/manual_008_profil.png)

Le bouton Modifier Profil permet de modifier les informations sur l’utilisateur courant :

![Menu User](/images/vitalis/manual_009_profil_form.png)

Modifier les informations sur vous 
* Noms et prénoms
* Changer la photo
* Mettre une petite description

**Changer mot de passe**

![Menu User](/images/vitalis/manual_010_profil_password.png)

**Autres menus**

* Paramètres : accessibles aux administrateurs
* Déconnexion: permettant de quitter l'application et retourner à l'écran de login

#### Ecrans et contenus

Voici les formes d'écrans et contenus visibles dans Vitalis.

**Type de Listing et tableaux**

Un écran présentant une liste : d’actes, de tâches ou autres données :
Exemple : une liste de demande de copies de naissance :

![Menu User](/images/vitalis/manual_011_ecrans_listing.png)

Pour accéder à un élément il faut cliquer sur la cellule de la première colonne de la ligne voulue.
Dans cet exemple il faut à la ligne voulue et cliquer sur le N° de reçu correspondant.
Dans une liste il y a :
* En titre : le nom de la liste
* Un paramètre de liste : afficher X par pages
* Un champ de recherche à droite
* L’entete du tableau de chaque colonne
* La liste des données
* En bas à droite des boutons de navigations par page de la liste.

**Avec recherche**

Dans toute liste, pour rechercher rapidement un acte ou une personne : tapez un bout d’information dans le champ de recherche, comme suit

![Listing avec recherche full-text](/images/vitalis/manual_012_ecrans_listing_search.png)

Vous pouvez y rentrer n’importe quelle information :
* Nom
* Numéro d’acte/tâches
* Date
* Nom de lieu
* …

**Ecran fiche de contenu**

En cliquant sur un élément, la fiche correspondante présentant le contenu de l’élément est affiché.
Ici les détails de l’acte et de la demande de copie :

![Fiche d'un document](/images/vitalis/manual_013_ecrans_fiche.png)

* Dans les cadres au milieu les informations sur l’acte
* Un cadre reservé à la demande ou déclaration
* En haut à gauche des boutons de traitement :
  * Aperçu : voir le rendu du document au format PDF
  * Valider : valider la saisie et les données : la demande/déclaration n’est plus modifiable
  * Modifier Acte : modifier le contenu de l’acte
  * Modifier fiche/tache : modifier la tâche en cours.

**Ecran de modification de l’acte**

Voici un exemple d’écran de modification d’acte

![Fiche d'un document](/images/vitalis/manual_014_ecrans_form.png)

**Ecran de modification de tâche**

Et pour le cas d’une demande de copie d’acte de naissance, l’écran matérialisant la demande :

![Fiche d'un document](/images/vitalis/manual_015_ecrans_form_demande.png)

Selon votre configuration, certaines informations ne seront pas affichées. Par exemple, les dates de fin de traitement et date de livraison.
* Le n° de reçu est un N° remis au demandeur/déclarant permettant de retrouver rapidement sa copie lors de la livraison. 
* Ce N° de reçu peut représenter aussi le reçu de paiement de tout droit applicable à la demande ou déclaration.7
* Signataire : en choisissant un signataire, le nom de celui-ci ainsi que sa fonction sera affiché en bas de l’acte imprimé. Sinon, il faudrait utiliser le tampon contenant son nom lors de la signature.