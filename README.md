# Projet de gestion d'un parc informatique : 

## 1) Présentation générale

Ce projet, nommé MyGestIOn'R, a pour objectif de simplifier la gestion du parc informatique pour les techniciens qui gère les système et réseau d'une entreprise. Il est développé en Bash et utilise une base de données MySQL pour stocker les informations essentielle d'un informaticien.

Ce document contient des informations sur la partie 1 du projet que j'ai réaliser, il se concentre sur la gestion de l'inventaire du parc informatique (ajouter, modifier, supprimer, etc. la base de donnée).

## 2) Détails des fonctionnalités

La première partie du projet "Gestion du parc informatique", permet de gérer l'inventaire des équipements de l'entreprise. Elle se constitue des éléments suivant :

* **Consulter les données** : Permet à l'utilisateur d'afficher les informations des équipements enregistrés dans la base de données MyGest. elle peux :
    * Afficher toutes les informations.
    * Afficher uniquement les machines.
    * Afficher uniquement les serveurs.
    * Afficher uniquement les switchs.
      
* **Ajouter des données** : Permet a utilisateur d'ajouter des équipements dans l'inventaire. Les informations nécessaire pour ajouter un équipement sont :
*  son adresse MAC (ex :00:1B:44:11:3A:B7).
*  son adresse IP (ex :192.168.16.24).
*  son masque de sous-réseau (ex :255.255.255.0).
*  son type (ex: machine, serveur ou switch).
  
* **Supprimer des données** : Permet a utilisateur de supprimer un équipement de l'inventaire comme ceci :
   * Entrer l'ID de l'équipement qu'il souhaite supprimer.
   * Le système affiche alors l'équipement qu'il a trouvé dans la base de donnée pour que l'utilisateur puisse le vérifier.
   * Une confirmation de suppression est demandée à l'utilisateur (en entrant 'y' pour oui ou 'n' pour non).
   * Si l'utilisateur confirme, l'équipement est supprimé de la base de données et un message de validation est affiché. Si l'utilisateur annule, aucune suppression n'est effectuée et un message d'annulation est affiché.

* **Modifier des données** : Permet aux utilisateurs de modifier les informations d'un équipement existant dans l'inventaire. Le processus de modification se déroule comme cela :
    * Entrer l'ID de l'équipement qu'il souhaite modifier.
    * Le système affiche alors les informations actuelles de cet équipement (ex : nom, adresse MAC, adresse IP, masque, type).
    * L'utilisateur dois ensuite saisir les nouvelles informations qu'il souhaite (si l'utilisateur ne souhaite pas modifier un champ, il le laisse vide).
    * Un message de confirmation est affiché une fois les informations de l'équipement mises à jour dans la base de données.
      

[**<ins>**Les choses que j'ai réalisées seul dans cette partie 1 sont :**</ins>**]

* **Consultation des données** : J'ai créer le script permettant d'interroger la base de données et d'afficher les informations des équipements selon l'option choisie par l'utilisateur.
* **Ajout de données** : J'ai créé un second script qui permet de saisir les informations d'un nouvel équipement et de les insérer dans la base de données.
* **Suppression de données** : J'ai ajouté une fonctionnalité qui permet de supprimer un une donnée de la base de données en fonction de l'ID de l'équipement.
* **Modification de donnée** : J'ai mis en place un processus qui permet de sélectionner un équipement par son ID, et de permettre à l'utilisateur de modifier ce qu'il souhaite.

## 3) La preuve en images : 

Voici quelques captures d'écran des script montrant les fonctionnalités que j'ai développées dans la partie "Gestion du parc" :

![image](https://github.com/user-attachments/assets/1b4c3122-7f6b-4dac-9450-8e7b1548a293)

*Script de consultation des données affichant la liste des équipements appelé "affiche.sh".*

![image](https://github.com/user-attachments/assets/be7e087c-2cff-4e1d-8000-b80c873a189b)
*Le formulaire de saisie des informations pour ajouter un nouvel équipement.*

![image](https://github.com/user-attachments/assets/cf926523-80e7-4560-8949-6934adc3346c)
*La confirmation de la suppression d'un équipement après avoir entré son ID.*

![image](https://github.com/user-attachments/assets/e715f736-a6d3-4cbb-bdde-a843b3b5614d)
*L'interface permettant de modifier les informations d'un équipement existant.*

## 4) Vidéo explicative : 
LIEN VIDEO A METTRE

Cette vidéo présente une démonstration des fonctionnalités de la partie "Gestion du parc" que j'ai réalisées. J'y explique un peu plus en détaille à quoi servent chaque éléments qui sont mis dans les scripts.

---___---  ** MERCI POUR VOTRE ATTENTION ! ** ---___---
