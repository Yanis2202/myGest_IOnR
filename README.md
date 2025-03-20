# Projet de gestion d'un parc informatique : 

## 1) Présentation générale

Ce projet, nommé MyGestIOn'R, a pour objectif de simplifier la gestion du parc informatique pour les techniciens qui gère les système et réseau d'une entreprise. Il est développé en Bash et utilise une base de données MySQL pour stocker les informations essentielle d'un informaticien.

Ce document contient des informations sur la partie 1 du projet que j'ai réaliser, il se concentre sur la gestion de l'inventaire du parc informatique (ajouter, modifier, supprimer, etc. la base de donnée).

## 2) Détails des fonctionnalités

La première partie du projet "Gestion du parc informatique", permet de gérer l'inventaire des équipements de l'entreprise. Il se constitue des éléments suivant :

* **Consulter les données** : Permet à l'utilisateurs d'afficher les informations des équipements enregistrés dans la base de données MyGest. elle peux :
    * Afficher toutes les informations.
    * Afficher uniquement les machines.
    * Afficher uniquement les serveurs.
    * Afficher uniquement les switchs.
      
* **Ajouter des données** : Permet aux utilisateurs d'ajouter des équipements dans l'inventaire. Les informations nécessaire pour ajouter un équipement sont :
*  son adresse MAC,
*  son adresse IP,
*  son masque de sous-réseau (CIDR)
*  son type (machine, serveur ou switch).
  
* **Supprimer des données** : Permet aux utilisateurs de supprimer un équipement de l'inventaire en spécifiant son identifiant unique (ID).
* **Modifier des données** : Permet aux utilisateurs de modifier les informations d'un équipement existant dans l'inventaire en spécifiant son ID. Les informations modifiables sont le nom, l'adresse MAC, l'adresse IP, le masque de sous-réseau (CIDR) et le type.

Les fonctionnalités que j'ai réalisées personnellement dans cette partie sont :

* **[**<ins>**Consultation des données**</ins>**]** : J'ai développé le script permettant d'interroger la base de données et d'afficher les informations des équipements selon les différentes options proposées.
* **[**<ins>**Ajout de données**</ins>**]** : J'ai créé le formulaire en ligne de commande qui permet de saisir les informations d'un nouvel équipement et de les insérer dans la base de données.
* **[**<ins>**Suppression de données**</ins>**]** : J'ai implémenté la fonctionnalité qui permet de supprimer un enregistrement de la base de données en fonction de l'ID de l'équipement.
* **[**<ins>**Modification de données**</ins>**]** : J'ai développé le processus qui permet de sélectionner un équipement par son ID, d'afficher ses informations actuelles et de permettre à l'utilisateur de modifier les champs souhaités avant de mettre à jour la base de données.

## 3) Mes réalisations

Voici quelques captures d'écran illustrant les fonctionnalités que j'ai développées dans la partie "Gestion du parc" :

![Capture d'écran de la consultation des données](lien_vers_votre_capture_consultation.png)
*L'interface de consultation des données affichant la liste des équipements.*

![Capture d'écran de l'ajout d'un équipement](lien_vers_votre_capture_ajout.png)
*Le formulaire de saisie des informations pour ajouter un nouvel équipement.*

![Capture d'écran de la suppression d'un équipement](lien_vers_votre_capture_suppression.png)
*La confirmation de la suppression d'un équipement après avoir entré son ID.*

![Capture d'écran de la modification d'un équipement](lien_vers_votre_capture_modification.png)
*L'interface permettant de modifier les informations d'un équipement existant.*

**(Note :** Veuillez remplacer les `lien_vers_votre_capture_...png` par les chemins d'accès réels aux captures d'écran que vous téléverserez dans votre dépôt GitHub. Pour cela, une fois les images téléversées, vous pourrez généralement cliquer dessus sur GitHub pour obtenir leur URL ou utiliser un chemin relatif si elles sont dans le même répertoire que le `README.md` ou dans un sous-répertoire.)

## 4) Démonstration technique

[Insérer ici le lien vers votre vidéo de présentation technique (voir Mission 2)]

Cette vidéo présente une démonstration des fonctionnalités de la partie "Gestion du parc" que j'ai réalisées. J'y montre comment consulter, ajouter, supprimer et modifier les informations des équipements dans la base de données MyGest.

## 5) Sources

* Le code source de la partie "Gestion du parc" est disponible dans ce dépôt GitHub. Il comprend les scripts Bash permettant d'interagir avec la base de données.
* Le fichier de base de données MySQL (`myGestI0nR.sql`) utilisé pour cette partie est également inclus dans ce dépôt.

---
