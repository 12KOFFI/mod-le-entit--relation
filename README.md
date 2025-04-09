# lien :  https://lucid.app/lucidchart/8513e62a-14b2-417d-93c4-155430df73dc/edit?beaconFlowId=5D8E1156B1DC3F40&invitationId=inv_a8370ca7-8107-4f26-a81c-fd14db7116c2&page=0_0#

📝 Présentation du Modèle Conceptuel de Données (MCD)
Ce MCD a été conçu dans le cadre d'une proposition de modernisation du système de gestion d’une chaîne de salles de sport. Actuellement, la gestion des inscriptions aux séances est manuelle, ce qui cause des erreurs et de l’insatisfaction client. L'objectif est de proposer une structure de base de données permettant une gestion numérique efficace des membres, des séances, des coachs et des gymnases.

🧩 Entités principales
Gymnase : Représente un établissement de sport, identifié par son nom, adresse et téléphone.

Membre : Personne inscrite dans un gymnase, avec des informations personnelles.

Coach : Encadrant sportif, spécialisé dans un type de sport.

Séance : Activité sportive proposée dans un gymnase à un horaire donné.

🔗 Relations
INSCRIRE : Un membre peut s’inscrire à plusieurs séances. Une séance peut accueillir jusqu’à 20 membres.

➤ Relation N:M

ANIMER : Un coach peut animer plusieurs séances. Une séance peut être animée par 1 à 2 coachs.

➤ Relation N:M (avec contrainte maximale)

APPARTIENT : Chaque membre est inscrit dans un seul gymnase. Un gymnase peut contenir plusieurs membres.

➤ Relation 1:N

ACCUEILLIR : Chaque séance a lieu dans un seul gymnase. Un gymnase peut accueillir plusieurs séances.

➤ Relation 1:N

🎯 Objectif du MCD
Le MCD permet de :

Suivre facilement les inscriptions des membres aux séances

Gérer la planification des coachs

Organiser les activités sportives par gymnase

Éviter les conflits de planning et d’inscription
