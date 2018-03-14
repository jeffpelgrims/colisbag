# MadaBag

## Le réseau d'échange pour envoyer et recevoir des colis de Madagascar

Développez par Pelgrims Jean-Francois

Design de la base de donnée
===========================

User => Par défaut les tables utilisées par Django
----

Profile => On va étendre les users avec cette table profile
-------
    Photo -- Photo de profil (not required)
    Tel_contact -- Un numéro de téléphone pour joindre 
    Ville -- Ville de résidence

Affiche => La table pour les affiches
-------
    Id_User_convoie
    Date_dep -- Date de départ
    Poids_disp -- Poids disponibles
    Poids_user -- Poids par personne
    Destination -- Ville de destination
    Information -- D'autres informations

Réservation => Table pour le formulaire de réservation
-----------
    Id_user_envoie
    Id_user_convoie
    Id_Affiche
    Poids_colis
    Desc_colis