@startuml
alt Supprimer un utilisateur
    Administrateur -> Système : Demande de suppresion de l'utilisateur
    Système -> Système : Suppression de l'utilisateur
    alt Erreur de suppression
       Système -> Administrateur : Affichage des erreurs
    else Pas d'erreur de suppression
       Système -> Administrateur : Affichage validation de suppression de l'utilisateur
    end 
else Modification d'un rôle
    Administrateur -> Système : Demande de l'ajout ou du retrait du rôle administrateur à un utilisateur
    Système -> Système : Enregistrement du rôle de l'utilisateur
    Système -> Administrateur : Affichage validation de l'ajout et duretrait du rôle
end
@enduml